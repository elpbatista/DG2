# 1. PDV 2: Definition Open Draft <!-- omit in toc -->

This is an enhanced version of [digital-guard](https://digital-guard.github.io/preservDataViz/src/preservCutGeo/index.html)

- [1. Requirements](#1-requirements)
  - [1.1. Functionalities Inherited from the Previous Version](#11-functionalities-inherited-from-the-previous-version)
  - [1.2. Design Features](#12-design-features)
  - [1.3. Technical Requirements](#13-technical-requirements)
- [2. Proposed Libraries](#2-proposed-libraries)
- [3. Roadmap](#3-roadmap)
  - [3.1. Stages](#31-stages)
  - [3.2. Estimated Labor](#32-estimated-labor)
- [4. References](#4-references)
  - [4.1. React Map Libraries](#41-react-map-libraries)
  - [4.2. React UI Libraries](#42-react-ui-libraries)
- [5. Notes](#5-notes)
- [6. Discussion](#6-discussion)
  - [6.1. Can Bootstrap been considered a lightweight library?](#61-can-bootstrap-been-considered-a-lightweight-library)
  - [6.2. Full screen map vs Horizontal split](#62-full-screen-map-vs-horizontal-split)
  - [6.3. Let's talk a little about the institutional websites ecosystem](#63-lets-talk-a-little-about-the-institutional-websites-ecosystem)

## 1. Requirements

### 1.1. Functionalities Inherited from the Previous Version

- [ ] Load GeoJSON files from GitHub [digital-guard / preservCutGeo-BR2021](https://github.com/digital-guard/preservCutGeo-BR2021/tree/main/data/MG/BeloHorizonte/_pk0008.01/geoaddress)
- [ ] Grayscale base map (default)
- [ ] Base map selector for: Google, Bing, OpenStreetMap
- [ ] Mosaic (choropleth map) with color by density
- [ ] Zoom level dependent labels
- [ ] Tooltips
- [ ] `on.click` in mosaics navigates to geohash's addresses
- [ ] Dot/Pin marker depending on the current zoom level
- [ ] Fixable popups with address details
- [ ] External toggles (fix-popups, remember-selection...)
- [ ] Geohash table with external selectors and column sorting
- [ ] Retrieve URL parameters in order to open the requested set of points (permalinks)
- [ ] Constrain the view to the bounding box of the mapped data
- [ ] Limited zoom-out

### 1.2. Design Features

- [ ] Single-page app
- [ ] _Full screen map vs Horizontal split_ still requires some [discussion]((#full-screen-map-vs-horizontal-split)) :point_up::cyclone:
- [ ] The design must comply with the **W3C standard.** A **flat design** and a **mobile-first** approach can also be used.

### 1.3. Technical Requirements

- [ ] React Web app that is suitable for desktop and mobile use
- [ ] Serverless application
- [ ] Integrate into an ecosystem of websites through [`react-router`](https://github.com/remix-run/react-router)
- [ ] The output of the components must be **Javascript-free,** pure HTML and CSS.

## 2. Proposed Libraries

Having done some research on the more established React projects for mapping and UI listed [below](#4-references), here is a _tentative proposal_ of libraries to use.

Mapping: [react-map-gl](https://github.com/visgl/react-map-gl) + [MapLibre](https://maplibre.org). See some examples [here](https://visgl.github.io/react-map-gl/example)

UI: [React Bootstrap](https://react-bootstrap.github.io)

## 3. Roadmap

This project is intended to be developed in the following 4 stages. Of course, they are open to discussion and modification if necessary.

### 3.1. Stages

1. **Design:** At this stage we should produce a set of agreed upon design concepts. It would be much better if it includes final sketches, mock-ups and proof-of-concepts. The effort should focus on creating a detailed feature list and "ideally" a very basic prototype of the future application.
2. **Development:** Coding, coding and more coding to obtain a fully functional application that implements all the features defined in the previous stage.
3. **Testing and Deployment:** This stage consists mainly of reviewing and testing all functionality from the client side (Peter) to find and fix bugs, errors and weaknesses that could affect the performance of the application in a production environment. When everyone is satisfied, the application will be ready for deployment.
4. **Maintenance:** Well, let's talk about future.

### 3.2. Estimated Labor

| stage | deliverables                   | hours  |
| :---: | ------------------------------ | :----: |
|   1   | App prototype, SRS + SOW       |   20   |
|   2   | Development App v0.x           |   40   |
|   3   | Production App v1.x            |   20   |
|   4   | Fixes and Updates App vx.x TBD |        |
|   -   | **Estimated time (hours):**    | **80** |

## 4. References

### 4.1. React Map Libraries

1. [deck.gl:](https://deck.gl) WebGL-powered framework for visual data analysis of large datasets. :+1: It is very memory-intensive. :-1:
2. [react-map-gl:](https://visgl.github.io/react-map-gl/) It is a suite of React components for Mapbox GL JS-compatible libraries. :+1: It also binds Mapbox GL forks like MapLibre. :+1:
3. [React Leaflet:](https://react-leaflet.js.org) React components for Leaflet maps. It's fine for very basic apps, but the interaction with map objects is too limited, just like Leaflet JS. :-1:
4. [React Simple Maps:](https://www.react-simple-maps.io) SVG maps developed in React with d3-geo and topojson. It focuses more on representation than analysis.

### 4.2. React UI Libraries

1. [MaterialUI:](https://mui.com) It is one of the best ReactJS UI frameworks. It is also the most popular React Component UI library. Data Grid components would need upgrade :moneybag: to PRO version. :-1:
2. [React Bootstrap:](https://react-bootstrap.github.io) **Bootstrap** is the most popular front-end framework, rebuilt for React. :+1:
3. [Ant Design:](https://ant.design) It provides a design system for enterprise products. React is used to encapsulate a library of components which embody its own design language. It adds an abstraction layer written in TypeScript to translate their design patterns into React components.

## 5. Notes

[Create React App](https://create-react-app.dev/docs/getting-started)

```text
npx create-react-app my-app
```

[react-router](https://github.com/remix-run/react-router)

```text
npm i react-router
```

[react-map-gl with MapLibre](https://visgl.github.io/react-map-gl/docs/get-started/get-started#using-with-a-mapbox-gl-fork)

```text
npm install --save react-map-gl maplibre-gl
```

## 6. Discussion

### 6.1. Can Bootstrap been considered a lightweight library?

Definitely not, but...

[Why React-Bootstrap?](https://react-bootstrap.github.io/getting-started/why-react-bootstrap/)

### 6.2. Full screen map vs Horizontal split

Please add your thoughts here

### 6.3. Let's talk a little about the institutional websites ecosystem

I will need a sketch to get an idea of where we are in this ecosystem. I'm already working on it.
