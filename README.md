# PrusaSlicer Configs for Creality Ender 3 Pro with Direct Drive

## Overview

This repository contains customized **PrusaSlicer 2.9.0** profiles for the **Creality Ender 3 Pro** with a **Direct Drive** modification. The profiles are specifically optimized for **Polymaker PolyTerra PLA+** filament, with the **0.2mm Normal profile** being extensively tested.

## Hardware Setup

The printer is equipped with the following modifications:

- **Printer:** Creality Ender 3 Pro
- **Direct Drive:** Custom Direct Drive conversion
- **Fan Mount:** [Thingiverse Link](https://www.thingiverse.com/thing:4369859)
- **BL-Touch Removed**: Manual bed leveling with paper method

## Included Configurations

The provided profile is optimized for Polymaker PolyTerra PLA+ filament:

| Profile               | Layer Height | Supported Nozzles | Tested |
| --------------------- | ------------ | ----------------- | ------ |
| **0.20 mm Normal**    | 0.20 mm      | 0.4 mm            | ✅      |

> **Note:** The **0.2mm Normal profile** has been extensively tested.

## 0.20mm Normal Profile Optimization

The following optimizations have been applied to the **0.2mm Normal profile**, specifically for **Polymaker PolyTerra PLA+** filament:

### **First Layer Settings:**
- First Layer Height: **0.24 mm**
- First Layer Speed: **20 mm/s**
- First Layer Extrusion Width: **0.44 mm**
- First Layer Temperature: **200°C**
- First Layer Bed Temperature: **65°C**

### **Retraction & Extrusion Settings:**
- Retraction Length: **1.3 mm**
- Retraction Speed: **50 mm/s**
- Retraction Before Wipe: **20%** (Previously 0.6%)
- Extrusion Multiplier: **1.01**
- Filament Diameter: **1.75 mm**
- Extrusion Width: **0.4 mm**

### **Additional Optimizations:**
- **Infill Density:** Increased from **15%** to **30%** for better structural integrity
- **Top Solid Layers:** Increased from **5** to **6** for improved top layer finish
- **Start GCode Optimization:**
  - Düse heizt erst auf **150°C**, dann erst auf Drucktemperatur → **Verhindert Filamentausfluss vor Druckbeginn**
  - **Erweiterte Reinigungslinien** für bessere Extrusionskontrolle
- **Seam Position:** Set to `Nearest`

## Installation

### 1. Importing PrusaSlicer Profiles

1. Open PrusaSlicer.
2. Go to **Settings → Import Profiles** and select `PrusaSlicer_config_bundle.ini`.
3. Enable the profile.

## License

These configuration files are provided under the **MIT License**, meaning you are free to use, modify, and share them.

## Feedback & Improvements

If you have suggestions for improvements or find any issues, feel free to create an issue on GitHub or submit a pull request with your adjustments.

