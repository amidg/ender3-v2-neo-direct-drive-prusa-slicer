# PrusaSlicer Configs for Creality Ender 3 Pro with Direct Drive

## Overview

This repository contains customized **PrusaSlicer 2.9.0** profiles for the **Creality Ender 3 Pro** with a **Direct Drive** modification. The profiles are optimized for **PLA+** filament, with the **0.2mm Normal profile** being extensively tested.

## Hardware Setup

The printer is equipped with the following modifications:

- **Printer:** Creality Ender 3 Pro
- **Fan Mount:** [Thingiverse Link](https://www.thingiverse.com/thing:4369859)
- **Direct Drive:** [Thingiverse Link](https://www.thingiverse.com/thing:4555065)
- **BL-Touch Mount:** [Thingiverse Link](https://www.thingiverse.com/thing:4823903)

## Included Configurations

The provided profiles include various print resolutions and optimizations for PLA+ filament:

| Profile               | Layer Height | Supported Nozzles | Tested |
| --------------------- | ------------ | ----------------- | ------ |
| 0.08 mm Superdetail   | 0.08 mm      | 0.4 mm            | ❌      |
| 0.10 mm Highdetail    | 0.10 mm      | 0.4 mm            | ❌      |
| 0.12 mm Detail        | 0.12 mm      | 0.4 mm            | ❌      |
| 0.16 mm Optimal       | 0.16 mm      | 0.4 mm            | ❌      |
| **0.20 mm Normal**    | 0.20 mm      | 0.4 mm            | ✅      |
| 0.24 mm Draft         | 0.24 mm      | 0.4 mm            | ❌      |
| 0.16 mm Optimal Speed | 0.16 mm      | 0.4 mm            | ❌      |
| 0.20 mm Normal Speed  | 0.20 mm      | 0.4 mm            | ❌      |
| 0.20 mm High Speed    | 0.20 mm      | 0.4 mm            | ❌      |

> **Note:** Only the **0.2mm Normal profile** has been extensively tested. All other profiles are available but not yet fully validated.

## 0.20mm Normal Profile Optimization

The following optimizations have been applied to the **0.2mm Normal profile**:

- **First Layer Settings:**
  - First Layer Height: 0.2 mm
  - First Layer Speed: 15 mm/s
  - First Layer Extrusion Width: 0.45 mm
  - First Layer Temperature: 205°C
  - First Layer Bed Temperature: 65°C
- **Retraction Settings:**
  - Retraction Length: 1.3 mm
  - Retraction Speed: 44 mm/s
  - Retraction Lift Z: 0.2 mm
- **Filament Flow & Extrusion Settings:**
  - Extrusion Multiplier: 1.00
  - Filament Diameter: 1.75 mm
  - Extrusion Width: 0.4 mm

## Installation

### 1. Importing PrusaSlicer Profiles

1. Open PrusaSlicer.
2. Go to **Settings → Import Profiles** and select either `PrusaSlicer_config_bundle.ini` or `config.ini`.
3. Enable the desired profile.

## License

These configuration files are provided under the **MIT License**, meaning you are free to use, modify, and share them.

## Feedback & Improvements

If you have suggestions for improvements or find any issues, feel free to create an issue on GitHub or submit a pull request with your adjustments.
