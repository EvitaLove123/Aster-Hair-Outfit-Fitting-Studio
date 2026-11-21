# Aster Hair & Outfit Fitting Studio

Android-friendly, browser-based VRM / GLB fitting preview.

## Current MVP (v0.1)
- Load a base character from VRM or GLB.
- Load separate hair and outfit accessories from VRM or GLB.
- Orbit, zoom, frame, show/hide, and manually adjust position, Y rotation, and uniform scale.
- Export the visible combined scene as **GLB**.
- Model files are processed locally in the browser; they are not uploaded to a server.

## Current limitations
- `.vroidcustomitem` is not supported yet. It requires a dedicated VRoid custom-item parser; renaming the file will not work.
- Accessories are independent scene objects. There is no automatic skeleton retargeting, skin-weight transfer, or mesh fitting yet.
- Export is GLB only. It is **not** a valid VRM 0.x or VRM 1.0 exporter.
- No UniVRM dependency and no fabricated UniVRM / UniGLTF metadata.

## Run
Open the GitHub Pages site in a modern browser with internet access (the Three.js and VRM libraries load from jsDelivr). Choose the base model first, then add accessories.

## Privacy
The model files are read locally by the browser. The site does not include an upload endpoint.
