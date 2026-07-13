# APT Disaster-Response & Rebuild Professionals

Public map of Association for Preservation Technology (APT) affiliated firms and individuals with
documented historic-preservation disaster-response and/or rebuild-phase experience.

Live at: https://rkn2.github.io/apt-disaster-response-map/

Built for APT's Disaster Response Initiative so that after a disaster, owners of historic buildings
can find nearby APT-affiliated professionals — both acute responders and the trades/firms who do the
historic rebuild once the rubble is cleared.

Color = what they do:
- **Purple** — documented acute disaster response experience *and* rebuild-phase specialty
- **Orange** — acute disaster responder only
- **Green** — rebuild-phase specialist only
- **Gray** — general preservation trade, no specific disaster/rebuild tag on file

Size = firm (larger) vs. individual (smaller).

Data: `data.geojson`, a public-safe copy of the full research dataset — name, location, firm-level
contact only (never personal), specialty/disaster tags, and cited past projects. Verification-status
notes and internal sourcing detail are stripped. Full research pipeline (331 records, source-cited,
historic-preservation gated) lives in a private repo; this repo exists only to publish this map.

Built with [Leaflet](https://leafletjs.com/) + OpenStreetMap tiles, no build step — just `index.html`
and `data.geojson`. Regenerate `data.geojson` from the private repo with
`python3 scripts/build_public_map.py path/to/this/repo/data.geojson`.
