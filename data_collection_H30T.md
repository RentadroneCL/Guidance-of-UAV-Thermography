# 📄 Data Collection Guide - Matrice 350 + DJI H30T

## 🎯 Objective
Thermographic inspection of photovoltaic (PV) plants with an IR resolution of **3 cm/pixel** and RGB resolution of **1 cm/pixel** using the DJI **H30T** payload on the Matrice 300/350 RTK drone.

---

## 🔧 Recommended Flight Parameters

| **Parameter**              | **IR Flight**                                | **RGB Flight**                             |
|---------------------------|----------------------------------------------|--------------------------------------------|
| **Sensor Used**           | Radiometric Thermal (1280×1024)              | Wide-angle RGB (48MP equiv. or better)     |
| **Resolution Target**     | 3 cm/pixel                                   | 1 cm/pixel                                  |
| **Flight Height (AGL)**   | ~80 m                                        | ~40 m                                       |
| **Flight Speed**          | 5 m/s                                        | 5 m/s                                       |
| **Front Overlap**         | 80%                                          | 80%                                         |
| **Side Overlap**          | 60%                                       | 70–80%                                      |
| **Camera Angle**          | Nadir (90°)                                  | Nadir (90°)                                 |
| **Trigger Mode**          | Time-based / Distance-based                  | Time-based / Distance-based                 |
| **Thermal Gain Mode**     | High-Res or Low Gain (based on environment)  | —                                           |
| **Emissivity**            | 0.95 (adjusted in post)                      | —                                           |
| **Reflective Temp.**      | 20–25°C (adjusted in post)                   | —                                           |
| **Ambient Temp. Source**  | External logger (if possible)                | —                                           |
| **Humidity Source**       | External logger (if possible)                | —                                           |
| **GeoTIFF Output**        | Enabled                                      | Enabled                                     |

---

## 🗺️ Flight Planning Tips

- Use **DJI Pilot 2** with DJI RC Plus for mission planning.
- Separate the IR and RGB flights for optimal resolution and focus.
- Fly during **consistent sun exposure** hours (10:00–15:00).
- Avoid cloud shadows and reflective glare.
- If using High-Res thermal mode, verify frame rate and coverage speed.

---

## 🧪 Post-Processing Notes

- IMPORTANT: Make sure the drone and camera are updated with the last available firmware, use DJI Assistant and check the DJI Official Drivers website.
- Use **DJI Thermal Analysis Tool 3** or **IRimage + Fiji** for radiometric R-JPEG to TIFF conversion.
- Confirm that all metadata (emissivity, gain, ambient temp) is accurate.
- Match RGB and IR flights by GPS data and timestamps for alignment.
