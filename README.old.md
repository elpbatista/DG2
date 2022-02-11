# PDV 2

This is an enhanced version of [digital-guard](https://digital-guard.github.io/preservDataViz/src/preservCutGeo/index.html)

## Requirements

- [ ] Load GeoJSON files from GitHub [digital-guard / preservCutGeo-BR2021](https://github.com/digital-guard/preservCutGeo-BR2021/tree/main/data/MG/BeloHorizonte/_pk0008.01/geoaddress)
- [ ] Grayscale base map (default)
- [ ] Base map selector for: Google, Bing, OpenStreetMap
- [ ] Mosaic (choropleth map) with color by density
- [ ] Zoom level dependent labels
- [ ] Tooltips
- [ ] `on.click` in mosaics navigates to geohash's addresses
- [ ] Dot/Pin marker depending on the zoom level
- [ ] Fixable popups with address details
- [ ] External toggles (fix-popups, remember-selection...)
- [ ] Geohash table with external selectors and column sorting
- [ ] React Web app that is suitable for desktop and mobile use
- [ ] Retrieve URL parameters in order to open the requested set of points  (permalinks)
- [ ] Constrain the view to the bounding box of the data
- [ ] Limit zoom-out

## Proposed Libraries

Mapping: [react-map-gl](https://github.com/visgl/react-map-gl) + [MapLibre](https://maplibre.org). See some examples [here](https://visgl.github.io/react-map-gl/example)

UI: [React Bootstrap](https://react-bootstrap.github.io)

## References

### React Map Libraries

1. [deck.gl:](https://deck.gl) WebGL-powered framework for visual data analysis of large datasets. :+1:
2. [react-map-gl:](https://visgl.github.io/react-map-gl/) It is a suite of React components for Mapbox GL JS-compatible libraries. :+1::+1:
3. [React Leaflet:](https://react-leaflet.js.org) React components for Leaflet maps.
4. [React Simple Maps:](https://www.react-simple-maps.io) SVG maps developed in React with d3-geo and topojson.

### React UI Libraries

1. [MaterialUI:](https://mui.com) It is one of the best ReactJS UI frameworks. It is also the most popular React Component UI library. Data Grid components need upgrade :moneybag: to PRO version. :skull_and_crossbones::-1:
2. [React Bootstrap:](https://react-bootstrap.github.io) **Bootstrap** the most popular front-end framework, rebuilt for React. :+1:
3. [Ant Design:](https://ant.design) It provides a design system for enterprise products. React is used to encapsulate a library of components which embody its own design language. It adds an abstraction layer written in TypeScript to translate their design patterns into React components.

## Notes

[react-map-gl with MapLibre](https://visgl.github.io/react-map-gl/docs/get-started/get-started#using-with-a-mapbox-gl-fork)

```text
npm install --save react-map-gl maplibre-gl
```
