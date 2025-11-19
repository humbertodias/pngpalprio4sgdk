[![CI](https://github.com/rahzelk/pngpalprio4sgdk/actions/workflows/ci.yml/badge.svg)](https://github.com/rahzelk/pngpalprio4sgdk/actions/workflows/ci.yml)
[![CD](https://github.com/rahzelk/pngpalprio4sgdk/actions/workflows/cd.yml/badge.svg)](https://github.com/rahzelk/pngpalprio4sgdk/actions/workflows/cd.yml)
![GitHub all releases](https://img.shields.io/github/downloads/rahzelk/pngpalprio4sgdk/total)

# PNG Palette and Priority Editor for SGDK  

PPP Editor for SGDK is a Java-based tool for editing palette and priority masks on indexed 8bpp PNG images, specifically designed for SGDK (Sega Genesis Development Kit) projects.

With PPP Editor, you can:  

✅ Load and visualize indexed 8bpp PNG images.<br/>
✅ Edit palette indices (0-3) and priority flags (0/1) on an 8×8 tile grid.<br/>
✅ Save this tile grid as a "mask" for future use<br/>
✅ Export the final image with the applied mask (=palette and priority encoding).<br/>
✅ Use a batch mode for automated processing via the command line.<br/>

## Known issues
The tool is rather slow with bigger image... got to improve this indeed !
PNG above 1024x1024 tends to be laggy...and higher resolution may become unusable.


## Installation & Usage
Need Java 8 (compiled with jdk1.8.0_441)

### GUI Mode : 

Download PPPE4SGDK.jar<br>
To show the GUI , simply run with Java: "java -jar PPPE4SGDK.jar"

### 🏭 Batch Mode (Command Line Processing)<br/>
Run the editor via the command line for automated processing:<br/>
java -jar PPPE4SGDK.jar --b <image_path> <mask_path> <export_path>

Example:<br/>
java -jar PPPE4SGDK.jar --b bgb.png mask.msk bgb_palprio.png



## Screenshots <br>
![screenshot](app_screenshot1.png)

## Features :

🎨 Image & Mask Handling<br/>
Load indexed 8bpp PNG images.<br/>
Save and load .msk mask files to preserve tile properties.<br/>

🖱️ Editing Capabilities<br/>
Left Click & Drag → Lasso selection of multiple tiles.<br/>
CTRL + Left Click → Add/remove multiple selection areas.<br/>
Right Click → Open a property editor to modify Palette index (0-3) and Priority (0 = low, 1 = high)<br/>

Keyboard Shortcuts:<br/>
H → Set priority High (1)<br/>
L → Set priority Low (0)<br/>
0, 1, 2, 3 → Change palette index of selected tiles<br/>
SHIFT + Mouse Wheel → zooming<br/>
Arrow Keys → Scroll image<br/>
CTRL+Z / CTRL+Y → undo / redo<br/>


## License <br>
This project is open-source under the MIT License.


