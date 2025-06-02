# 📄 Data Collection Guide - DJI Matrice 4T

## 🎯 Objective
Thermographic inspection of photovoltaic (PV) plants with an IR resolution of **3 cm/pixel** and RGB resolution of **1 cm/pixel** using the DJI **Matrice 4T** drone.

---

## 🔧 Recommended Flight Parameters

| **Parameter**              | **IR Flight**                  | **RGB Flight**                 |
|---------------------------|-------------------------------|-------------------------------|
| **Sensor Used**           | Radiometric Thermal (640×512) | Wide-angle RGB (48MP equiv.)  |
| **Resolution Target**     | 3 cm/pixel                    | 1 cm/pixel                    |
| **Flight Height (AGL)**   | ~55 m                         | ~40 m                         |
| **Flight Speed**          | 5 m/s                         | 5 m/s                         |
| **Front Overlap**         | 80%                           | 80%                           |
| **Side Overlap**          | 60%                        | 70–80%                        |
| **Camera Angle**          | Nadir (90°)                   | Nadir (90°)                   |
| **Trigger Mode**          | Time-based / Distance-based   | Time-based / Distance-based   |
| **Thermal Gain Mode**     | Low Gain (recommended)        | —                             |
| **Emissivity**            | 0.95 (adjusted in post)       | —                             |
| **Reflective Temp.**      | 20–25°C (adjusted in post)    | —                             |
| **Ambient Temp. Source**  | External logger (if possible) | —                             |
| **Humidity Source**       | External logger (if possible) | —                             |
| **GeoTIFF Output**        | Enabled                       | Enabled                       |

---

## 🗺️ Flight Planning Tips

- Use **DJI Pilot 2** app for flight mission creation.
- Separate the IR and RGB flights to ensure proper resolution goals.
- Plan flights during **low wind conditions** and with **consistent sunlight**.
- If possible, fly **between 10:00–15:00** to ensure panel heating.
- Avoid strong reflections and cloud shadows.

---

## 🧪 Post-Processing Notes

- IMPORTANT: Make sure the drone is updated with the last available firmware, use DJI Assistant and check the DJI Official Drivers website.
- Use **DJI Thermal Analysis Tool 3** or **IRimage + Fiji** for radiometric TIFF conversion.
- Ensure all metadata (flight altitude, timestamp, emissivity) is correctly applied.
- Match RGB and IR datasets by timestamp and GPS data for precise overlay.
