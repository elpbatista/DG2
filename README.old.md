# 1. PDV 2 <!-- omit in toc -->

This is an enhanced version of [digital-guard](https://digital-guard.github.io/preservDataViz/src/preservCutGeo/index.html)

- [1.1. Requirements](#11-requirements)
- [1.2. Proposed Libraries](#12-proposed-libraries)
- [1.3. Roadmap](#13-roadmap)
  - [Stages](#stages)
  - [Estimated Labor](#estimated-labor)
- [1.4. References](#14-references)
  - [1.4.1. React Map Libraries](#141-react-map-libraries)
  - [1.4.2. React UI Libraries](#142-react-ui-libraries)
- [1.5. Notes](#15-notes)

## 1.1. Requirements

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
- [ ] Retrieve URL parameters in order to open the requested set of points (permalinks)
- [ ] Constrain the view to the bounding box of the data
- [ ] Limit zoom-out

## 1.2. Proposed Libraries

Mapping: [react-map-gl](https://github.com/visgl/react-map-gl) + [MapLibre](https://maplibre.org). See some examples [here](https://visgl.github.io/react-map-gl/example)

UI: [React Bootstrap](https://react-bootstrap.github.io)

## 1.3. Roadmap

### Stages

1. Design
2. Development
3. Testing and deployment
4. Maintenance

### Estimated Labor

| stage | deliverables              | time / hours |
| :---: | ------------------------- | -------------- |
|   1   | App mockups, SRS + SOW    |                |
|   2   | Development App v0.x      |                |
|   3   | Production App v1.x       |                |
|   4   | Updated Versions App vx.x |                |

## 1.4. References

### 1.4.1. React Map Libraries

1. [deck.gl:](https://deck.gl) WebGL-powered framework for visual data analysis of large datasets. :+1: It is very memory-intensive. :-1:
2. [react-map-gl:](https://visgl.github.io/react-map-gl/) It is a suite of React components for Mapbox GL JS-compatible libraries. :+1: It also binds Mapbox GL forks like MapLibre. :+1:
3. [React Leaflet:](https://react-leaflet.js.org) React components for Leaflet maps. It's fine for very basic apps, but the interaction with map objects is too limited, just like Leaflet JS. :-1:
4. [React Simple Maps:](https://www.react-simple-maps.io) SVG maps developed in React with d3-geo and topojson. It focuses more on representation than analysis.

### 1.4.2. React UI Libraries

1. [MaterialUI:](https://mui.com) It is one of the best ReactJS UI frameworks. It is also the most popular React Component UI library. Data Grid components need upgrade :moneybag: to PRO version. :skull_and_crossbones::-1:
2. [React Bootstrap:](https://react-bootstrap.github.io) **Bootstrap** the most popular front-end framework, rebuilt for React. :+1:
3. [Ant Design:](https://ant.design) It provides a design system for enterprise products. React is used to encapsulate a library of components which embody its own design language. It adds an abstraction layer written in TypeScript to translate their design patterns into React components.

## 1.5. Notes

[react-map-gl with MapLibre](https://visgl.github.io/react-map-gl/docs/get-started/get-started#using-with-a-mapbox-gl-fork)

```text
npm install --save react-map-gl maplibre-gl
```
