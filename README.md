# PrusaSlicer Configs for Creality Ender 3 V2 Neo with Direct Drive

> 🔎 Keywords: PrusaSlicer Profile, Creality Ender 3 V2 Neo, Direct Drive, Creality PLA, 3D Printing, Misfeed Prevention, Optimized Profiles

## Overview

This repository contains **customized PrusaSlicer 2.9.1** profiles specifically designed for the **Creality Ender 3 V2 Neo** with **Direct Drive** modification. These profiles are optimized for **Creality's own PLA filament** with a primary focus on **minimizing misfeeds** and ensuring reliable, consistent printing performance.

**🔗 Based on the excellent work from:** [s3vdev/PrusaSlicer-Profiles-Ender3Pro-DirectDrive](https://github.com/s3vdev/PrusaSlicer-Profiles-Ender3Pro-DirectDrive)

## Key Differences from Original Project

While this project is inspired by the original Ender 3 Pro profiles, it has been **completely rewritten** for the Ender 3 V2 Neo with significant optimizations:

### **Hardware Differences:**
- **Printer:** Ender 3 V2 Neo (220x220x250mm build volume)
- **Direct Drive:** Default stepper motor with default gears
- **Nozzle:** 0.4mm standard nozzle
- **Bed Leveling:** Manual leveling with 0.203mm feeler gauge
- **Filament:** Creality PLA (vs. original Polymaker PolyTerra PLA+)

### **Primary Focus - Misfeed Prevention:**
- **Ultra-conservative retraction settings** (0.8mm @ 35mm/s)
- **Reduced accelerations** for smoother filament flow
- **Pressure stabilization pauses** in start G-code
- **Multi-stage heating sequences** to prevent oozing
- **Gentle prime sequences** with small test extrusions

---

## Hardware Setup

The printer configuration these profiles are designed for:

* **Printer:** Creality Ender 3 V2 Neo
* **Build Volume:** 220 x 220 x 250 mm
* **Direct Drive:** Stock Ender 3 V2 Neo direct drive system
* **Stepper Motor:** Default Creality stepper
* **Gears:** Default gear ratio
* **Nozzle:** 0.4mm standard nozzle
* **Bed Leveling:** Manual leveling using 0.203mm feeler gauge
* **Filament:** **Creality PLA** (optimized for Creality's own filament)

> ⚠️ **Important:** These profiles are specifically tuned for **Creality PLA filament** and **direct drive systems**. While they may work with other PLA brands, optimal results are achieved with Creality's filament.

---

## Included Configurations

### Print Profiles (Anti-Misfeed Optimized)

| Profile Name                    | Layer Height | Speed Focus | Optimized For                    | Support Coverage |
| ------------------------------- | ------------ | ----------- | -------------------------------- | ---------------- |
| **Ender3V2Neo QUALITY 0.15mm** | 0.15 mm      | Slow        | High-detail prints, small parts  | Ultra-dense      |
| **Ender3V2Neo NORMAL 0.20mm**  | 0.20 mm      | Balanced    | General purpose printing         | Dense            |
| **Ender3V2Neo DRAFT 0.28mm**   | 0.28 mm      | Fast        | Rapid prototyping, large parts   | Standard         |

### Filament Profile
- **Creality PLA Ender3V2Neo DirectDrive**: Optimized specifically for Creality PLA with conservative extrusion settings

### Printer Profile
- **Creality Ender3V2Neo DirectDrive 0.4mm**: Complete printer definition with anti-misfeed G-code sequences

---

## Anti-Misfeed Optimizations

### **Retraction Settings (Critical for Direct Drive):**
- **Retraction Length:** 0.8mm (significantly reduced from Bowden systems)
- **Retraction Speed:** 35mm/s (conservative to prevent jamming)
- **Z-Lift:** 0.1mm (minimal to prevent excessive movement)
- **Only retract when crossing perimeters:** Enabled

### **Temperature Management:**
- **Printing Temperature:** 205°C (conservative for reliable flow)
- **First Layer Temperature:** 210°C (higher for better adhesion)
- **Bed Temperature:** 60°C (65°C first layer)
- **Idle Temperature:** 160°C (prevents oozing during pauses)

### **Bed Leveling & First Layer:**
- **Manual Bed Leveling:** Calibrated with 0.203mm feeler gauge
- **First Layer Height:** 0.203mm (matches feeler gauge for perfect adhesion)
- **Consistent Across Profiles:** All quality settings use same first layer height
- **Perfect Bed Contact:** No floating first layers or poor adhesion

### **Speed & Acceleration (Smooth Filament Flow):**
- **First Layer Speed:** 15-20mm/s (extra slow for reliability)
- **External Perimeter Speed:** 20-30mm/s (conservative)
- **Default Acceleration:** 300-500mm/s² (reduced from typical 1000+)
- **Travel Speed:** 150mm/s (moderate to reduce vibration)

### **Enhanced G-Code Sequences:**
- **Multi-stage heating:** Prevents filament oozing during startup
- **Pressure stabilization pauses:** Allows filament pressure to equalize
- **Conservative prime lines:** Gentle extrusion testing before print
- **Gentle retracts:** Small test retracts to ensure proper feeding

---

## Support Material Enhancements

### **Maximum Coverage Support System:**
- **Automatic Support Generation:** Always enabled
- **Support Spacing:** 0.2mm (ultra-dense for complete coverage)
- **Pattern:** Rectilinear (most reliable)
- **Contact Distance:** 0.3mm (easy removal with good support)
- **XY Spacing:** 40% (adequate clearance from part walls)
- **Threshold:** 35° (aggressive overhang detection)
- **Support from anywhere:** Not limited to buildplate only

### **Fan Settings for Optimal Cooling:**
- **Fan Speed:** 100% throughout entire print
- **Fan Activation:** Layer 2 (immediate cooling)
- **Bridge Fan Speed:** 100% (maximum cooling for overhangs)

---

## 🚀 Quick Start Guide

### 1. Import the Configuration Bundle

1. Download `PrusaSlicer_config_bundle_ender3v2neo_creality_pla.ini`
2. Open **PrusaSlicer 2.9.1** or newer
3. Go to **File → Import → Import Config Bundle**
4. Select the downloaded `.ini` file
5. All profiles will be imported automatically

### 2. Select Your Profile

Choose based on your printing needs:
- **QUALITY (0.15mm):** For detailed miniatures, small mechanical parts
- **NORMAL (0.20mm):** For most general printing tasks *(recommended starting point)*
- **DRAFT (0.28mm):** For quick prototypes and large structural parts

### 3. Load Your Model and Print

1. Import your STL/3MF file
2. Supports will generate automatically for any overhangs >35°
3. Slice and print with confidence - the profiles handle misfeed prevention automatically

---

## Expected Print Quality & Performance

### **Reliability Improvements:**
✅ **Drastically reduced misfeeds** - Conservative settings prevent jamming  
✅ **Consistent extrusion** - Pressure management prevents flow variations  
✅ **Automatic support coverage** - No manual support adjustment needed  
✅ **Clean overhangs** - 100% fan cooling provides excellent overhang quality  

### **Print Quality:**
✅ **Smooth surface finish** - Conservative speeds reduce vibration artifacts  
✅ **Strong layer adhesion** - Optimized temperatures for Creality PLA  
✅ **Reliable first layers** - Slow, controlled first layer deposition  
✅ **Easy support removal** - 0.3mm contact distance balances support and removal  

### **Performance Characteristics:**
- **Print Speed:** Moderate (prioritizes reliability over speed)
- **Material Usage:** Slightly higher (dense supports for reliability)
- **Success Rate:** Very high (conservative settings prevent failures)
- **Maintenance:** Low (reduced wear from gentle operation)

---

## Troubleshooting & Fine-Tuning

### **If you still experience misfeeds:**
- Reduce retraction length to 0.6mm
- Increase printing temperature by 5°C
- Check filament path for obstructions

### **If you see stringing:**
- Increase retraction length to 1.0mm (but keep speed at 35mm/s)
- Ensure 100% fan speed is active
- Check nozzle temperature isn't too high

### **For different PLA brands:**
- Adjust temperature ±10°C based on manufacturer recommendations
- Fine-tune extrusion multiplier (start with 0.95-1.02 range)
- Test retraction settings on small calibration prints

### **Bed Leveling Calibration:**
- **Use 0.203mm feeler gauge** for consistent bed leveling
- **All profiles use 0.203mm first layer height** - no profile-specific adjustments needed
- **If using different gauge thickness:** Update `first_layer_height` values in all three print profiles
- **Perfect adhesion indicator:** First layer should stick without gaps or over-squishing

---

## Comparison with Original Project

| Aspect                  | Original (Ender 3 Pro)        | This Project (Ender 3 V2 Neo)     |
| ----------------------- | ----------------------------- | ---------------------------------- |
| **Primary Focus**       | Print quality optimization    | **Misfeed prevention**            |
| **Filament**           | Polymaker PolyTerra PLA+      | **Creality PLA**                  |
| **Retraction**         | Standard direct drive         | **Ultra-conservative (0.8mm)**    |
| **Supports**           | Manual configuration          | **Automatic, ultra-dense**        |
| **Cooling**            | Variable fan speed            | **100% fan always**               |
| **Print Speed**        | Balanced                      | **Conservative for reliability**   |
| **Target Users**       | General 3D printing           | **Users experiencing misfeeds**   |

---

## Contributing & Feedback

These profiles were developed through extensive testing specifically for the Ender 3 V2 Neo with direct drive. If you have suggestions for improvements or encounter issues:

1. **Create an issue** describing your problem and printer setup
2. **Submit a pull request** with tested improvements
3. **Share your results** to help improve the profiles for everyone

---

## License

This project is provided under the **MIT License** - feel free to use, modify, and share these configurations.

---

## Acknowledgments

**Special thanks to [s3vdev](https://github.com/s3vdev)** for the original [PrusaSlicer-Profiles-Ender3Pro-DirectDrive](https://github.com/s3vdev/PrusaSlicer-Profiles-Ender3Pro-DirectDrive) project that served as the foundation and inspiration for this work. While this project has been completely rewritten for different hardware and objectives, the original project provided valuable insights into direct drive optimization.

---

**Happy printing with your Ender 3 V2 Neo! 🚀**  
*No more misfeeds, just reliable prints.*