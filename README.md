# exif_inspect

**exif_inspect** is a pure HTML+JavaScript tool for inspecting the EXIF metadata of image files, including GPS coordinates plotted on Google Maps. No backend, no Python — just drop it in a browser and go.

## Features

- Drag-and-drop interface for image files
- Extracts and displays:
  - Camera make, model, and exposure info
  - Timestamps
  - GPS latitude/longitude (if available)
  - Image orientation, resolution, and more
- Displays geotagged locations on an embedded Google Map
- All client-side — nothing is uploaded or stored

## Requirements

- A modern web browser (Chrome, Firefox, Edge, Safari)
- A [Google Maps JavaScript API key](https://developers.google.com/maps/documentation/javascript/get-api-key)

## Setup

1. Clone or download this repo.
2. Open `exif.html` in a text editor.
3. Replace the placeholder in the Google Maps script tag with your actual API key:

```html
<script async defer src="https://maps.googleapis.com/maps/api/js?key=YOUR_GOOGLE_MAPS_API_KEY&callback=initMap"></script>

