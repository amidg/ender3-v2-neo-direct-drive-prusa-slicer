# PrusaSlicer Configs for Creality Ender 3 Pro with Direct Drive
> 🔎 Keywords: PrusaSlicer Profile, Creality Ender 3 Pro, Direct Drive, Polymaker PolyTerra PLA+, 3D Printing, Best Settings, Optimized Profiles

## Overview

This repository contains customized **PrusaSlicer 2.9.1** profiles for the **Creality Ender 3 Pro** with a **Direct Drive** modification. The profiles are specifically optimized for **Polymaker PolyTerra PLA+** filament, with separate configurations for **small** and **large** prints to ensure optimal results for various model sizes.

## Hardware Setup

The printer is equipped with the following modifications:

- **Printer:** Creality Ender 3 Pro
- **Direct Drive:** [Ender 3 V2 Direct Drive](https://www.thingiverse.com/thing:4555065)
- **Fan Mount:** [Thingiverse Link](https://www.thingiverse.com/thing:4369859)
- **BLTouch (Antclabs) Removed**: Manual bed leveling using the paper method
- **Filament:** **Polymaker PolyTerra PLA+**

> ⚠️ **Important:** While these profiles are optimized for **Polymaker PolyTerra PLA+**, they may also work well with other PLA+ filaments. However, adjustments to temperatures, retraction settings, or cooling might be necessary for best results.

---

## Included Configurations

The provided profiles are optimized for **Polymaker PolyTerra PLA+** filament and differentiated for small and large prints:

| Profile                     | Layer Height | Infill Density | Optimized For | Tested |
|-----------------------------|---------------|-----------------|----------------|---------|
| **0.20 mm Normal (LARGE)**   | 0.20 mm       | 30%             | Large, stable models | ✅ |
| **0.20 mm Normal (SMALL)**   | 0.20 mm       | 15%             | Small, detail-focused models | ✅ |
| **0.16 mm Normal (LARGE)**   | 0.16 mm       | 20%             | High-detail large models | ✅ |

> **Note:** All profiles have been tested extensively for quality and reliability.

---

## Optimizations & Key Features

### **First Layer Settings (All Profiles):**
- First Layer Height: **0.24 mm** (LARGE) / **0.20 mm** (SMALL) / **0.24 mm** (0.16 mm LARGE)
- First Layer Speed: **20 mm/s**
- First Layer Extrusion Width: **0.48 mm** (LARGE) / **0.45 mm** (SMALL) / **0.48 mm** (0.16 mm LARGE)
- First Layer Temperature: **200°C**
- First Layer Bed Temperature: **65°C**

### **Retraction & Extrusion Settings:**
- Retraction Length: **1.3 mm** (LARGE) / **1.0 mm** (SMALL) / **1.2 mm** (0.16 mm LARGE)
- Retraction Speed: **50 mm/s**
- Retraction Before Wipe: **20%** (LARGE) / **0.6%** (SMALL) / **15%** (0.16 mm LARGE)
- Extrusion Multiplier: **1.01**
- Filament Diameter: **1.75 mm**
- Extrusion Width: **0.4 mm**

### **Additional Optimizations:**
- **Infill Density:**  
  - **30%** for LARGE profile to improve structural stability  
  - **15%** for SMALL profile to reduce material usage and printing time  
  - **20%** for 0.16 mm LARGE profile for improved structural detail
- **Top Solid Layers:**  
  - **6** for LARGE prints to ensure strong, smooth top layers  
  - **5** for SMALL prints to optimize print speed
- **Start GCode Optimization:**  
  - Düse heizt erst auf **150°C**, dann auf Drucktemperatur → **Verhindert Filamentausfluss vor Druckbeginn**
  - **Erweiterte Reinigungslinien** für verbesserte Extrusionskontrolle
- **Seam Position:** Set to `Nearest` for reduced visible seams.

---

## 🚀 Quick Start

### 1. Importing PrusaSlicer Profiles
1. Open **PrusaSlicer**.
2. Go to **Settings → Import Profiles** and select `PrusaSlicer_config_bundle-combi.ini`.
3. Select the desired profile depending on your print size:
   - **LARGE** for big, stable parts.
   - **SMALL** for smaller, detail-oriented prints.
   - **0.16 mm LARGE** for higher detail on large parts.
4. Use **200°C nozzle temperature** and **65°C bed temperature** for optimal results.

---

## Tips for Best Results
✅ Use the **LARGE** profile for big models to ensure better stability and layer adhesion.  
✅ Use the **SMALL** profile for smaller parts where precision and detail are critical.  
✅ Use the **0.16 mm LARGE** profile for complex models requiring higher detail.  
✅ All profiles are optimized to reduce **stringing** and **warping**, which were common issues in earlier configurations.  

![Preview | width=400](Preview.JPEG)
---

## License

These configuration files are provided under the **MIT License**, meaning you are free to use, modify, and share them.

---

## Feedback & Improvements

If you have suggestions for improvements or find any issues, feel free to create an **issue** on GitHub or submit a **pull request** with your adjustments.

Enjoy smooth and reliable prints! 🚀
