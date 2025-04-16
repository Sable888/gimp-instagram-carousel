📦 GIMP Plugin Pack - Installation & Usage Guide

---

🗂 Where to Place These Files:

1. Click the Windows **Start/Search bar**.
2. Type:
   %appdata%\GIMP\3.0\plug-ins
3. Press Enter.

⚠️ If the `plug-ins` folder doesn’t exist, you can create it manually.

4. Paste all the plugin folders/files here from this ZIP.

🚫 **Do not remove or separate the `.py` files from their folders.**
Each plugin must stay inside its own correctly named folder to work properly in GIMP.

---

📁 Additional Files to Place in Documents:

In addition to the plugins, you should also place the following files in your **Documents** folder for easier access:

1. `instagram_canvas_preset.xcf`  
   - This is your wide Instagram layout canvas (21600 x 1350).  
   - You will open this in GIMP when starting a new carousel layout.

2. `instagram_tiff_export.batcher.json`  
   - This is the export preset used by the Batcher plugin.  
   - You can load this preset inside the Batcher interface to export your slices as high-quality TIFFs directly into the Documents folder.

🪄 How to do it:
- Press **Win + R**, type `Documents`, and hit Enter.
- Move the `.xcf` and `.json` files into this folder manually.

---

🖼 How to Use in GIMP:

1. Launch GIMP 3.0.
2. Open the included `.xcf` file — this is the **wide canvas preset** (21600 x 1350) used to align and preview Instagram carousel layouts.
   - You can move this `.xcf` file to your `Documents` folder for easier access.
   - If you make changes to it, **use "Save As"** to avoid overwriting the original canvas preset.

3. Import your images:
   - Go to **File > Open as Layers...**
   - Select multiple images to load them into the canvas as separate layers.
   - ⚠️ **Importing TIFFs may take a little extra time**, but using TIFF is essential to preserve HDR image quality.

4. Use the tools in this order (found under the **Guides** menu):

   - **Add Guides** – Inserts vertical guide lines spaced for 4:5 Instagram slicing.
   - **Auto Scale** – Resizes each layer to fit the full height of the canvas (1350px), but does **not** automatically position them.
     - After scaling, you must manually move each image to your preferred layout using the Move Tool.
   - **Slice It** – Cuts the canvas into evenly spaced slices using the guides.
   - **Export** – Saves each slice as a separate image file.

---

💾 Export Tips:

- TIFF is preferred for HDR quality preservation.
- JPEG is available via alternate plugin if needed.
- You can use the included `instagram_tiff_export.batcher.json` preset with the Batcher plugin to export images directly to your **Documents** folder.

---

🛠 GIMP Installation:

If GIMP 3.0 is not installed, run the included installer:
▶ `gimp-3.X.X-setup.exe`

Or download the latest version at:
🔗 https://www.gimp.org/downloads/devel/

---

🧼 Troubleshooting:

If the plugins don’t show up:
- Make sure they’re in this folder: `%appdata%\GIMP\3.0\plug-ins`
- ✅ Ensure each `.py` file is **inside the folder it came in**, not dragged out
- Restart GIMP after copying the files
- Windows handles permissions automatically for `.py` files

---

🧠 Advanced Notes:

- These plugins use the GIMP 3.0 Python system.
- Fully tested for layout, slicing, and exporting workflows.
- No additional setup or configuration required.
