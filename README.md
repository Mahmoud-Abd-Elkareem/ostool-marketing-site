# Ostool marketing site

Public product site for Ostool — a single static page (`index.html`, no build step)
introducing the fleet-maintenance platform, embedding a recorded tour of the
Operations portal (`journey.webm` / `poster.png`), and a contact form that posts
to the FleetMaintenance backend's public contact endpoint.

## Running locally

Open `index.html` directly in a browser, or serve the folder with any static
file server, e.g.:

```
npx serve .
```

## Contact form

The form posts to `POST /api/public/contact` on the FleetMaintenance API
(see `FleetMaintenance-refactored-v3`). Update the `API_BASE` constant near
the top of the `<script>` block in `index.html` to point at your API's URL
(defaults to `http://localhost:5000` for local development).
