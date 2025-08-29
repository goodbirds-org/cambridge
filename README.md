# Goodbirds Cambridge

Automated Folium maps of eBird “Notable” observations within 20 km of Cambridge, MA.

- Center: 42.378500, -71.115600
- Rings at 5, 10, 15, 20 km
- Runs twice daily and on demand with GitHub Actions
- Publishes to GitHub Pages at https://goodbirds-org.github.io/cambridge/

## Setup
1. Add repo secret `EBIRD_API_KEY` with your eBird key.
2. Place `goodbirds_logo_text.png` at repo root. The workflow copies it to `docs/`.
3. Enable GitHub Pages: Settings → Pages → Build from `/docs`.
4. Run the “Build Cambridge Map” action.

Output:
- `docs/index.html` archive
- `docs/maps/<timestamp>.html` timestamped maps
- `docs/maps/latest.html` convenience link
