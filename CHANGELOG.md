# Changelog

All notable changes to this project will be documented in this file.

## [iri-0.0.0] - 2023-03-14

### Change

- IRI fork: call invalidateSize when map component gets resized.

## [0.1.25] - 2022-07-20

### Change

- Leaflet and react-leaflet are now [bundled with dash-leaflet](https://github.com/thedirtyfew/dash-leaflet/pull/146). This structure enables **development of plugins as external packages**. 
- Various dependency updates.

## [0.1.23] - 2021-08-11

### Change

- Changed loading of js chunks so that a chunk is only loaded when actually needed.

## [0.1.22] - 2021-08-11

### Added

- Added [`Minichart component`](https://github.com/thedirtyfew/dash-leaflet/pull/116).

### Changed

- The following components are now loaded async: `EditControl`, `GeoTIFFOverlay`, `LocateControl`, `MeasureControl`, `MarkerClusterGroup`. As a result, the main bundle size has been reduced to about half (< 500 kB).
- Update to Dash 2.0.
- Prop validation of `GeoJSON` component `hideout` prop relaxed.
- Prop validation of `Polygon` component `positions` prop relaxed.

## [0.1.18] - 2021-02-09

### Added

- Added `drawToolbar` and `editToolbar` props to `EditControl` component.

### Changed

- Polygons collected into the `geojson` prop of the `EditControl` component are now closed.

## [0.1.16] - 2021-07-07

### Added

- Added `EditControl` component.
- Added `GestureHandling` component.
- Fixing [issue](https://github.com/thedirtyfew/dash-leaflet/issues/95)
- Fixing [issue](https://github.com/thedirtyfew/dash-leaflet/issues/96)

## [0.1.15] - 2020-17-06

### Added

- New `FeatureGroup` component.

### Changed

- Fixed bug in `GeoJSON` component arising when all features are filtered out and `zoomToBounds=True`.

### Removed

- Dropped bundled js functions (previously located in `express.js`).

## [0.1.14] - 2020-17-06

### Added

- Added `extraProps` prop to `WMSTileLayer` component as per [request](https://github.com/thedirtyfew/dash-leaflet/issues/90).

## [0.1.13] - 2020-13-01

### Added

- Added `layers` prop to `LayersControl` component.
- Added `FullscreenControl` as per [request](https://github.com/thedirtyfew/dash-leaflet/issues/67).

## [0.1.12] - 2020-12-12

### Changed

- Regression (bounds passed from Dash not applied) due to fix in 0.1.11 [fixed](https://github.com/thedirtyfew/dash-leaflet/issues/62)

## [0.1.11] - 2020-04-12

### Changed

- New attempt at fixing a [bug](https://github.com/thedirtyfew/dash-leaflet/issues/56) typically seen with multiple maps in multiple tabs.

## [0.1.10] - 2020-27-11

### Changed

- Breaking syntax changes in functional properties.

## [0.1.8] - 2020-20-11

### Changed

- Fixed a [bug](https://github.com/thedirtyfew/dash-leaflet/issues/56) typically seen with multiple maps in multiple tabs.

## [0.1.7] - 2020-14-11

### Added

- Added [MeasureControl](https://github.com/thedirtyfew/dash-leaflet/pull/50).

## [0.1.5] - 2020-20-10

### Added

- Added EasyButton component.
- Added tracking of map bounds.

## [0.1.4] - 2020-23-09

### Added

- The LayersControl has (finally) been added.

### Changed

- Minor changes to GeoJSON standard functions adding support for discrete/continuous color scales for both scatter and choropleth

## [0.1.3] - 2020-17-09

### Added

- The map now supports [different CRS](https://github.com/thedirtyfew/dash-leaflet/issues/31).
- The GeoJSON component now [supports custom panes](https://github.com/thedirtyfew/dash-leaflet/issues/38).
- The GeoJSON now supports [changing style dynamically](https://github.com/thedirtyfew/dash-leaflet/issues/42).

## [0.1.1] - 2020-04-09

### Changed

- The MarkerClusterGroup is again included for backwards compatibility
- Per default, the GeoJSON now renders tooltip/popup if a `tooltip`/`popup` property is available on the feature
- The GeoJSON example functions (scatter, choropleth) have been moved from Python to JavaScript thus eliminating the dash-transcrypt dependency

## [0.1.0] - 2020-03-09

### Added

- New geojson subpackage. It contains modules with examples of python function definitions to ease the transition to functional props

### Changed

- The GeoJSON has been completely rewritten to support a wider range of use cases. It now uses functional props

### Removed

- The SuperCluster component has been removed. The GeoJSON component now handles marker clustering

## [0.0.22] - 2020-30-07

### Changed

- Supercluster: spiderfy bug fixed, added automatic maxZoom detection

## [0.0.21] - 2020-24-07

### Added

- Added Supercluter component.

## [0.0.20] - 2020-09-07

### Added

- Added tracking of map zoom and center.
- Added tracking marker position.
- Added build instructions to readme.

## [0.0.19] - 2020-09-07

### Added

- Added some build automation (github actions).

## [0.0.18] - 2020-22-06

### Changed

- Fix of bug in Polygon prop validation.
- Added DivMarker component.

## [0.0.17] - 2020-19-05

### Changed

- Pane component bug fixed.
- Verification of scrollWheelZoom type corrected.

## [0.0.16] - 2020-20-05

### Added

- Pane component added.

## [0.0.15] - 2020-19-05

### Changed

- PolylineDecorator component properties "positions" and "children" changed to dynamic.

## [0.0.14] - 2020-17-05

### Added

- PolylineDecorator component added.

## [0.0.13] - 2020-11-05

### Changed

- Options property added to MarkerClusterGroup.

## [0.0.12] - 2020-11-05

### Changed

- Property added to GeoJSON object (n_click).
- Link added to heroku documentation.

## [0.0.11] - 2020-11-05

### Changed

- GeoJSON object added.

## [0.0.10] - 2020-06-05

### Changed

- Support of multiple urls for VideoOverlay

## [0.0.9] - 2020-28-04

### Added

- ScaleControl object added.



## [0.0.8] - 2020-22-04

### Changed

- Property added to Map to signal location change (location_lat_lon_acc)
- CircleMarker changed to use n_clicks like Marker
- New options added to LocateControl

## [0.0.7] - 2020-17-04

### Added

- LocationControl object added.

## [0.0.6] - 2020-16-04

### Added

- MarkerClusterGroup object added.

## [0.0.5] - 2020-11-04

### Changed

- Click event for Marker object change from yielding (lat, lon) to n_clicks to ensure that the event fires on each click.

## [0.0.4] - 2020-10-04

### Added

- Click event for Marker object added.
