# 🖼️ GIMP Instagram Carousel Plugins

A collection of custom GIMP 3.0 plugins for streamlined Instagram carousel creation — including layout, slicing, and high-quality export with TIFF support.

---

## 📦 Plugin Contents

- `instagram_add_19_guides.zip`  
  Adds 19 vertical guides to a 21600×1350 canvas for 20-image Instagram carousels.

- `slice_by_guides.zip`  
  Uses GIMP's built-in guillotine slicing to split the image along guides.

- `Scale_and_Center_Layers.zip`  
  Automatically scales each layer to fit vertically within the canvas (1350px tall).  
  Does **not** reposition or spread layers horizontally — placement must still be done manually.

- `batcher.zip`  
  A slightly tweaked version of the open-source **Batcher** plugin for export.  
  - ❗ **Menu location changed**: The "Useful Tool" button now appears under the **Guides** menu (instead of its original location) to match the rest of this plugin suite.

- `instagram_tiff_export.batcher.json`  
  A preconfigured export profile for use with Batcher. Exports sliced images as `.TIFF` to preserve HDR quality.

- `21600×1350 canvas.xcf`  
  A base canvas template matching Instagram’s vertical 4:5 aspect ratio.

- `INSTALL_README.txt`  
  Installation instructions for users.

---

## 🧩 Requirements

- GIMP 3.0+
- Python 3.12 or later
- Recommended: [Batcher Plugin](https://github.com/kamilburda/batcher) for export automation

---

## 📤 Exporting with Batcher

This plugin set uses a customized version of the [Batcher plugin by kamilburda](https://github.com/kamilburda/batcher) to automate exporting Instagram carousel slices as TIFF files.

> ⚙️ **Tweak Note**: The Batcher plugin included in this repo has been modified to move the **Useful Tool** menu under **Guides**, keeping all Instagram-related tools in one place.

To use:
1. Install Batcher (included in this repo).
2. Launch it via **Guides → Useful Tool**.
3. Import the provided `.json` export profile.
4. Use Quick Export to save all slices as high-quality `.TIFF`.

---

## 🛠️ Installation

1. Extract each `.zip` folder into your GIMP plugins directory:
