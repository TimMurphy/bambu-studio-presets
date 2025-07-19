# 🎛️ Bambu A1 3D Print Presets Repository

This repository contains version-controlled configurations for 3D printing with the Bambu A1. It manages filament profiles, slicing workflows, printer setups, calibration models, and annotated results—structured for reproducibility, version tracking, and workshop insights.

## 🔄 Exporting Presets from Bambu Studio

Use `File → Export → Export Preset Bundle…` to generate and save configuration files. Below are the five available export types—presented in the order shown in Bambu Studio—and instructions for organizing each in this repo.

Always export to the `\exported-presets` folder.

### Printer preset bundle (`.bbscfg`)

Exports a complete printer configuration, including linked filament and process presets. Ideal for backing up your Bambu A1 setup or restoring full configurations.

### Filament preset bundle (`.bbsflmt`)

Exports a single filament profile with customized parameters—temperature, flow rate, retraction, cooling—tailored by color, nozzle, or brand.

### Printer presets (`.zip`)

Batch-export individual printer presets in a zipped archive (usually containing JSON files).

Unzip the exported archive before committing to maintain version control visibility. Extract all files to the `\exported-presets\Printer presets\` folder, then delete the original `.zip` file. Individual JSON files provide better diff tracking and merge resolution than compressed archives.

### Filament presets (`.zip`)

Batch-export multiple filament presets in one zipped bundle.

Unzip the exported archive before committing to maintain version control visibility. Extract all files to the `\exported-presets\Filament presets\` folder, then delete the original `.zip` file. Individual JSON files provide better diff tracking and merge resolution than compressed archives.

Unzip before committing. Place extracted files in `\filaments`.

### Process presets (`.zip`)

Exports slicing process profiles (layer height, speed, ironing, wall settings, supports, infill).

Unzip the exported archive before committing to maintain version control visibility. Extract all files to the `\exported-presets\Process presets\` folder, then delete the original `.zip` file. Individual JSON files provide better diff tracking and merge resolution than compressed archives.

## 📦 Additional Folders

These folders are not exported directly by Bambu Studio but support calibration, benchmarking, and documentation for repeatable print testing and evaluation.

### \test-models-and-results

**Description:**  

Contains test models and their associated results—grouped by filename for contextual clarity. Each print experiment includes the model file (`.stl`, `.3mf`) and related assets such as analysis logs or photos.

#### 🧪 Test Models

Below is a categorized list of recommended test models to include in `\test-models-and-results`. These files support benchmarking, tuning, and visual comparisons across filament, process, and printer presets.

---

TODO

---

**Maintainer:** Tim  
**Printer:** Bambu A1  
**Tools Used:** Bambu Studio, Fusion 360, Git, Copilot