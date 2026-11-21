# Aster Hair & Outfit Fitting Studio

Android-friendly, browser-based VRM / GLB fitting preview.

## Features
- Load a base character from VRM or GLB.
- Load separate hair and outfit accessories from VRM or GLB.
- Orbit, zoom, frame, show/hide, and adjust position, rotation, and scale.
- Transform gizmo with Move / Rotate / Scale modes.
- List and delete individual meshes from the base character; undo the last deletion.
- Export the visible scene as GLB.
- Export VRM 0.x or VRM 1.0 when the base character is a VRM. The VRM exporter is a separate MIT-licensed open-source module; see `VRMExporter-LICENSE.txt`.
- Model files are processed locally in the browser; they are not uploaded to a server.

## Limitations
- A GLB-only base character cannot be exported as VRM by this workflow.
- Accessories are added as scene objects. They are not automatically rigged, retargeted, or skin-weighted to the base skeleton. Validate exported VRMs in your target app.
- `.vroidcustomitem` export is not supported. Valid custom items require VRoid Studio-specific item data such as category, parameters, texture-layer information, and format version. Renaming a GLB/VRM file is not a conversion.
- No UniVRM dependency and no fabricated UniVRM / UniGLTF metadata.

## Run
Open the GitHub Pages site in a modern browser with internet access (Three.js and VRM libraries load from jsDelivr). Choose the base model first, then add accessories.

## Privacy
The model files are read locally by the browser. The site does not include an upload endpoint.
