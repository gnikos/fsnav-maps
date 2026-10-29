# fsnav-maps

Starter sea maps for the FSN boat app (https://app.fsnav.gr/), served at https://maps.fsnav.gr/.
Catalog version: 2026-10-29.

**Όχι για ναυσιπλοΐα / Not for navigation.**
Οι χάρτες αυτοί δεν είναι για ναυσιπλοΐα. / These maps are an aid for fishing, not a nautical chart.

## Files

- `regions.json` - the catalog: the overview and each region (id, name, outline polygon, file names, sizes, version).
- `*-base.pmtiles` - base maps (land, coast, places) as PMTiles, Protomaps vector tiles (schema v4). Readable by MapLibre,
  QGIS and https://pmtiles.io/. `overview-base.pmtiles` covers all of Greece; the others are detailed regions.
- `*-depths.json` - depth lines as GeoJSON. Each feature has the properties `d` (depth in metres) and `k`
  (`'fill'` = a depth area, `'line'` = a depth contour line). `overview-depths.json` covers all of Greece.
- `island-names.json` - the named islands and islets of Greece (OpenStreetMap place=island / islet) as GeoJSON points
  with `n` (the name, Greek first) and `z` (the zoom it shows from).

## Sources and licences

- Base maps © OpenStreetMap contributors (ODbL), built by Protomaps.
- Depth lines derived from EMODnet Bathymetry Consortium (2024): EMODnet Digital Bathymetry (DTM), CC BY 4.0.
- Overview depth lines derived from GEBCO Compilation Group (2026) GEBCO 2026 Grid.

Όχι για ναυσιπλοΐα / Not for navigation.
