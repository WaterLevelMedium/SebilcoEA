# Changelog

#### *for* Sebilco Environmental Assessment WebMap
- The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)
_____
*All notable changes to this project will be documented in this file.*

## [Unreleased]


## [0.1.0] - 2023-02-03
### Added
- SSURGO flood max layers for the primary site
- toggle checkboxes for primary ssurgo. Template formed
- panTo behavior on Dropdown click
- style handling functions for the primary_SSURGO_Flood Frequency layer as the proprties names vary slightly between geojson datasets for each site.
### Fixed
- Projection issues with the primary_SSURGO layer. Did not transform to WGS84 during export from QGIS.
- Sidebar checkbox toggle behavior. Checkboxes still have state issues, i.e., 'checked' or not. Will fix after all pertinent layers are uploaded as the user can visually tell if the layer is present or not
- Created helper function to bypass map.panTo(layer.getLat... too finicky writing each one out. Try Catch block allows both polygon geojson layers and markers.

### Removed
- Search bar at the Bottom. Have nothing to query.
- Unnecessary list items in each dropdown

### Changed
- Put offcanvas sidebar at bottom of page for better visibility of each layer

## [0.0.3] - 2023-02-02
### Added
- Organized dropdowns in offcanvas. Added toggle checkboxes and fixed behavior of toggleLayer()
- Added Hwy 226 facility polygons, classified SSURGO flood frequency layers
### Changed
- Simplified general site popup format
### Fixed
- Leaflet from 1.8.0 > 1.9.3


## [0.0.2] - 2023-02-01
### Added
- Created changeLog
- Clarified comments for helper functions and sectioned layer groups
## [0.0.2] - 2023-01-30
### Added
- Added SSURGO Data for Schoolhouse Dr, organized the layers.
- Added google maps links in the popup

### Fixed
- Chroma 1.3.4 > Chroma 2.4.2
- JQuery 3.6.1 > 3.6.3
- Bootstrap 4.0.0 > 5.3.0

## [0.0.1] - 2023-01-28

### Added
- Created webmap from elements of 'Mine Sites' and 'SecurityCamLocator'
- Added NCDOT_County_Boundaries_Spat.geojson to assets.
### Fixed
- Some Libraries


----
# Libraries

| Name | Date | Old Ver# | New Ver# | Old CDN | New CDN |
|----|----|----|----|---|---|---|
| Bootstrap | 2023-02-01 | 4.0.0 | 5.3.0 |    ` <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous"> <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.0.0/dist/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script> ` |   ` <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous"> <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js" integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script> ` |
|Empty Placeholder|||||||
| Chroma | 2023-02-01 | 1.3.4 | 2.4.2 | ` <script src="https://cdnjs.cloudflare.com/ajax/libs/chroma-js/1.3.4/chroma.min.js"></script> ` | `<script src="https://cdnjs.cloudflare.com/ajax/libs/chroma-js/2.4.2/chroma.min.js" integrity="sha512-zInFF17qBFVvvvFpIfeBzo7Tj7+rQxLeTJDmbxjBz5/zIr89YVbTNelNhdTT+/DCrxoVzBeUPVFJsczKbB7sew==" crossorigin="anonymous" referrerpolicy="no-referrer"></script> ` |\
|Empty Placeholder|||||||
| JQuery | 2022-02-01 | 3.6.1 | 3.6.3 | `<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.1/jquery.min.js"></script>`| `<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.3/jquery.min.js" integrity="sha512-STof4xm1wgkfm7heWqFJVn58Hm3EtS31XFaagaa8VMReCXAkQnJZ+jEy8PCC/iT18dFy95WcExNHFTqLyp72eQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script> `|
| JQuery | 2022-10-13 | 3.1.0 | 3.6.1 | `  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.0/jquery.min.js"></script> ` | `  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.1/jquery.min.js"></script>`| `<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.3/jquery.min.js" integrity="sha512-STof4xm1wgkfm7heWqFJVn58Hm3EtS31XFaagaa8VMReCXAkQnJZ+jEy8PCC/iT18dFy95WcExNHFTqLyp72eQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script> ` |
|Leaflet| 2023-02-02 | 1.8.0 | 1.9.3| `<link rel="stylesheet" href="https://unpkg.com/leaflet@1.8.0/dist/leaflet.css" integrity="sha512-hoalWLoI8r4UszCkZ5kL8vayOGVae1oxXe/2A4AO6J9+580uKHDO3JdHb7NzwwzK5xr/Fs0W40kiNHxM9vyTtQ=="crossorigin=""/> <script src="https://unpkg.com/leaflet@1.8.0/dist/leaflet.js" integrity="sha512-BB3hKbKWOc9Ez/TAwyWxNXeoV9c1v6FIeYiBieIWkpLjauysF18NzgR1MBNBXf8/KABdlkX68nAhlwcDFLGPCQ=="crossorigin=""></script>`| `<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.9.3/leaflet.css" integrity="sha512-mD70nAW2ThLsWH0zif8JPbfraZ8hbCtjQ+5RU1m4+ztZq6/MymyZeB55pWsi4YAX+73yvcaJyk61mzfYMvtm9w==" crossorigin="anonymous" referrerpolicy="no-referrer" /> <script src="https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.9.3/leaflet.js" integrity="sha512-Dqm3h1Y4qiHUjbhxTuBGQsza0Tfppn53SHlu/uj1f+RT+xfShfe7r6czRf5r2NmllO2aKx+tYJgoxboOkn1Scg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>`
