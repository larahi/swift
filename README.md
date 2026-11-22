# Alpine Swift Colony Monitoring

A lightweight static web portal for collecting and viewing alpine swift colony
field data in Switzerland.

## Features

- Upload one or more colony data photos.
- Record egg-nest, egg-size, nestling, and sampling-list observations.
- Select the monitored colony and observation date.
- Automatically generate consistent filenames for uploaded photos.
- View monitored colonies on an interactive Leaflet map.
- Open the shared Google Drive folder for uploaded records.

## Running locally

This is a static site and does not require a build step. Serve the repository
with any local web server, then open `index.html`:

```bash
python3 -m http.server
```

The upload form sends images to the configured Google Apps Script endpoint.
Update `UPLOAD_ENDPOINT` in `index.html` if the backend changes.

## Deployment

Pushes to the `main` branch are deployed to GitHub Pages by
`.github/workflows/static.yml`.

## Credits

The visual theme is based on
[Massively by HTML5 UP](https://html5up.net/massively), licensed under the
Creative Commons Attribution 3.0 license. Map tiles are provided by
[OpenStreetMap](https://www.openstreetmap.org/) through
[Leaflet](https://leafletjs.com/).
