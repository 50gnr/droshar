---
{"dg-publish":true,"dg-permalink":"atlas","permalink":"/atlas/","dg-note-properties":{}}
---


<div id="map" style="height: 75vh; width: 100%; border-radius: 8px;"></div>

<link
  rel="stylesheet"
  href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
/>

<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>

<script>
(async function () {
  const data = await fetch("/img/droshar-leaflet.json").then(r => r.json());

  const bounds = data.mapViewParameters?.bounds || [[0, 0], [3276, 4096\|0, 0], [3276, 4096]];
  const imageUrl = "/img/Droshar.jpg";

  const map = L.map("map", {
    crs: L.CRS.Simple,
    minZoom: -2.5,
    maxZoom: 2,
    zoomSnap: 0.5
  });

  L.imageOverlay(imageUrl, bounds).addTo(map);
  map.fitBounds(bounds);

  function findMarkers(obj) {
    const found = [];

    function walk(value) {
      if (Array.isArray(value)) {
        value.forEach(walk);
        return;
      }

      if (value && typeof value === "object") {
        if (value.loc && value.link) found.push(value);
        Object.values(value).forEach(walk);
      }
    }

    walk(obj);
    return found;
  }

  function slugify(name) {
    return name
      .normalize("NFD").replace(/[\u0300-\u036f]/g, "")
      .toLowerCase()
      .replace(/['’]/g, "")
      .replace(/[^a-z0-9]+/g, "-")
      .replace(/^-+|-+$/g, "");
  }

  const markers = findMarkers(data);
  console.log("Droshar markers found:", markers.length);

  markers.forEach(marker => {
    const pin = L.marker(marker.loc).addTo(map);

    const label = marker.link;
    const url = `/notes/${slugify(label)}/`;

    pin.bindPopup(`<a href="${url}">${label}</a>`);
  });
})();
</script>