# Super Traverse

A browser superhero-traversal game built on real-world map data. Swing, wall-crawl and web-zip through real cities, with rooftop freeflow combat. Tuned for a phone plus Bluetooth controller.

**Play:** https://jonmortensen12.github.io/super-traverse/

## Places
The default city is downtown Salt Lake City, built in. Tap **Choose place** to search anywhere on Earth, pick a skyline preset, or use your location. The game downloads that area's OpenStreetMap data (via the free Overpass service) and builds the city; each place is saved on the device after the first download.

## What the city is built from
- Buildings, streets, parks and trees from OpenStreetMap, including real heights and roof shapes (pyramids, spires, domes).
- Real ground elevation from the free AWS Terrain Tiles, loaded in the browser at startup.
- Optional USGS aerial mode (United States): public-domain USDA NAIP aerial photos on the ground and projected onto roofs, on the game's own clean geometry.
- Optional photoreal visuals from Google Photorealistic 3D Tiles. By default you also collide with the Google mesh itself, using live raycasts against the tiles on screen (nothing is saved or rebuilt from Google's data). Height is aligned automatically against street level.

## Google 3D tiles
1. Open **Map settings** on the start screen.
2. Paste your Google Map Tiles API key and tap **Save key**. It is stored only in that browser, never in this repository.
3. Tap **Google 3D tiles**. The page reloads with photoreal visuals.
4. Height is aligned automatically. If something still looks off, pause the game and use **Google tiles alignment**. To collide with OpenStreetMap shapes instead of the Google mesh, turn off **Collide with Google 3D mesh** in Map settings.

Each page load with Google tiles on uses one billable session (1,000 free per month).

## Credits
- Map data © OpenStreetMap contributors, available under the Open Database License (ODbL).
- Aerial imagery: USDA NAIP via USGS The National Map (public domain).
- Elevation: Terrain Tiles on AWS (Mapzen terrain, including USGS 3DEP data).
- Photorealistic 3D Tiles © Google Maps Platform, shown with Google's on-screen attribution.
- Rendering: three.js, NASA-AMMOS 3DTilesRendererJS and three-mesh-bvh. Place search: Nominatim. Map picker: Leaflet.
