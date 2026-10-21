# Super Traverse

A browser superhero-traversal game built on real-world map data. Swing, wall-crawl and web-zip through real cities, with rooftop freeflow combat. Tuned for a phone plus Bluetooth controller.

**Play:** https://jonmortensen12.github.io/super-traverse/

## Current build: downtown Salt Lake City
- Buildings, streets, parks and trees from OpenStreetMap, including real heights and roof shapes (pyramids, spires, domes).
- Real ground elevation from the free AWS Terrain Tiles, loaded in the browser at startup.
- Optional photoreal visuals from Google Photorealistic 3D Tiles. OpenStreetMap shapes stay underneath as invisible collision.

## Google 3D tiles
1. Open **Map settings** on the start screen.
2. Paste your Google Map Tiles API key and tap **Save key**. It is stored only in that browser, never in this repository.
3. Tap **Google 3D tiles**. The page reloads with photoreal visuals.
4. If the tiles sit too high or low, or look rotated, pause the game and use **Google tiles alignment**. **Show collision shapes** overlays the OpenStreetMap buildings so you can line them up.

Each page load with Google tiles on uses one billable session (1,000 free per month).

## Credits
- Map data © OpenStreetMap contributors, available under the Open Database License (ODbL).
- Elevation: Terrain Tiles on AWS (Mapzen terrain, including USGS 3DEP data).
- Photorealistic 3D Tiles © Google Maps Platform, shown with Google's on-screen attribution.
- Rendering: three.js and NASA-AMMOS 3DTilesRendererJS.
