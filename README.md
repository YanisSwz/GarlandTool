# Garland Tool

A Scriptable Tool for Unreal Engine that places a garland actor with an
editable spline and an attached PCG graph, which uses a data asset to generate elaborated decorations.

![Demo](./Visuals/Tool1.gif?raw=true)

## Requirements
- Unreal Engine 5.6.x (built and tested on 5.6.1)
- This plugin automatically enables its required engine plugins on activation:
  - Scriptable Tools Editor Mode
  - Scriptable Tools Framework
  - Modeling Tools Editor Mode
  - PCG
  - PCG Geometry Script Interop

## Installation
1. Download or clone this repo.
2. Copy the `GarlandTool` folder into your project's `Plugins/` directory
   (create the folder if it doesn't exist).
3. Restart the editor. You may be prompted to enable the plugin, choose Yes.
4. <b>No compiling required, this is a 100% Blueprint / content-only plugin.</b>

### Alternative: git submodule
If your project is already a git repo: </br>
git submodule add https://github.com/YanisSwz/GarlandTool Plugins/GarlandTool

## Usage

A detailed tutorial is available in PDF, it explains how to create data assets used by the tool, and how to use the tool.

### Garland Tool
1. In the viewport toolbar, open the **Selection Mode** dropdown and choose
   **Scriptable Tools**.
2. Find **Garland Tool** in the tool palette under the **Misc** category.
3. Setup the variables: the cord's mesh, and the Data asset to use for decorations along the garland.
![Demo](./Visuals/ToolDetails.png?raw=true)
4. Click/drag in the viewport to place the garland.
5. The placed actor already has a PCG graph attached and will generate
   automatically along the spline.

### Data Asset

The tool uses a Data asset to generate decorations along the garland. Read the tutorial to learn more about its content.

![Demo](./Visuals/DataAssetDetails.png?raw=true)

## Examples
![Demo](./Visuals/Tool1.gif?raw=true)
![Demo](./Visuals/Tool2.gif?raw=true)
![Demo](./Visuals/Tool3.gif?raw=true)

## License
MIT