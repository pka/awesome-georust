# Awesome Geo Rust [![awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

[<img src="https://georust.org/logo.png" align="right" width="100">](https://georust.org/)

> A curated list of awesome geospatial software, libraries, tools and resources, written in Rust

[Rust](https://www.rust-lang.org/), a language empowering everyone
to build reliable and efficient software.

Contributions welcome. Add links through [pull requests](https://github.com/pka/awesome-georust/pulls) or create an [issue](https://github.com/pka/awesome-georust/issues) to start a discussion. Please take a look at the [contribution guidelines](CONTRIBUTING.md).

## Contents

- [Awesome Geo Rust](#awesome-geo-rust-)
    - [Geospatial primitives and algorithms](#geospatial-primitives-and-algorithms)
    - [Handling GIS data formats](#handling-gis-data-formats)
    - [Raster and image processing](#raster-and-image-processing)
    - [OSM data handling](#osm-data-handling)
    - [Spatial index / Search](#spatial-index--search)
    - [3D](#3d)
    - [Geocoding](#geocoding)
    - [Routing](#routing)
    - [Web Services](#web-services)
    - [Map rendering](#map-rendering)
    - [Applications](#applications)
    - [Watchlist](#watchlist)
- [Resources](#resources)
    - [Community](#community)

### Geospatial primitives and algorithms
* [Geo](https://github.com/georust/geo) - Geospatial primitives such as Point & LineString, and algorithms such as distance, convex hull, centroidcalculations.
* [GEOS](https://github.com/georust/geos) - Bindings for the Geometry Engine - Open Source (GEOS) library.
* [Robust](https://github.com/georust/robust) - Robust primitives for computational geometry.
* [PROJ](https://github.com/georust/proj) - Bindings for the PROJ library for coordinate transformation and projections.
* [geographiclib-rs](https://github.com/georust/geographiclib-rs) - A port of geographiclib (geodesic calculations).
* [S2](https://github.com/danhhz/s2) - S2 spherical geometry library in Rust.
* [rust-geo-booleanop](https://github.com/21re/rust-geo-booleanop) - Rust implementation of the Martinez-Rueda Polygon Clipping Algorithm.
* [intersect2d](https://github.com/eadf/intersect2d.rs) - Line intersection sweep-line algorithm.
* [spatial-join](https://github.com/msalib/spatial-join) - Perform streaming geospatial-joins on geographic data.
* [tile-grid](https://crates.io/crates/tile-grid) - Library for map tile grid calculations.
* [zonebuilder](https://github.com/zonebuilders/zonebuilder-rust) - Build zones for large geographic regions.
* [Polylabel-rs](https://github.com/urschrei/polylabel-rs) - A Rust implementation of the Polylabel algorithm, with FFI.

### Spatial index / Partioning
* [rstar](https://github.com/georust/rstar) - R\*-tree library for the rust ecosystem.
* [kdbush](https://github.com/pka/rust-kdbush) - A Rust port of kdbush, a fast static spatial index for 2D points.
* [spade](https://github.com/Stoeoef/spade) - Delaunay Triangulations for the Rust ecosystem.
* [delaunator-rs](https://github.com/mourner/delaunator-rs) - A very fast static 2D Delaunay triangulation library for Rust.
* [earcutr](https://github.com/donbright/earcutr) - Port of MapBox's earcut triangulation code to Rust language.
* [boostvoronoi](https://github.com/eadf/boostvoronoi.rs) - Segmented Voronoi for Rust.

### Handling GIS data formats
* [GDAL](https://github.com/georust/gdal) - Bindings for the Geographic Data Abstraction Library (GDAL) for reading and writing raster and vector GIS files.
* [GeoZero](https://github.com/georust/geozero) - Zero-Copy reading and writing of geospatial data.
* [GeoJSON](https://github.com/georust/geojson) - Work with GeoJSON files.
* [GPX](https://github.com/georust/gpx) - Work with GPS files.
* [kml](https://github.com/georust/kml) - Rust support for reading and writing KML.
* [GeoTIFF](https://github.com/georust/geotiff) - Work with GeoTIFF raster files.
* [image-tiff](https://github.com/image-rs/image-tiff) - TIFF decoding and encoding library in pure Rust.
* [netCDF](https://github.com/georust/netcdf) - Bindings for Network Common Data Form (netCDF) library. Can read and write HDF5 files.
* [hdf5-rust](https://github.com/aldanor/hdf5-rust) - Thread-safe Rust bindings and high-level wrappers for the HDF5 library API.
* [N5](https://github.com/aschampion/rust-n5) - N5 "Not HDF5" tensor file system format.
* [shapefile-rs](https://github.com/tmontaigu/shapefile-rs) - Rust library to read & write shapefiles.
* [TileJSON](https://github.com/georust/tilejson) - Work with TileJSON files.
* [Transit](https://github.com/georust/transitfeed) - Work with GTFS files.
* [WKT](https://github.com/georust/wkt) - Work with Well-Known Text (WKT) files.
* [World file](https://github.com/georust/world-file) - Work with World-files.
* [FlatGeobuf](https://github.com/flatgeobuf/flatgeobuf) - A performant binary encoding for geographic data based on flatbuffers.
* [las-rs](https://github.com/gadomski/las-rs) - Read and write ASPRS las files.
* [stac-rs](https://github.com/gadomski/stac-rs) - Rust implementation of the SpatioTemporal Asset Catalog (STAC) specification.

### Raster and image processing
* [rasters.rs](https://github.com/AspecScire/rasters.rs) - Raster processing library and tools written in rust.
* [geo-rasterize](https://github.com/msalib/geo-rasterize/) - A pure-rust 2D rasterizer for geospatial applications.

### OSM data handling
* [osmpbfreader-rs](https://github.com/TeXitoi/osmpbfreader-rs) - Read OpenStreetMap PBF files.
* [osmpbf](https://github.com/b-r-u/osmpbf) - Library for reading the OpenStreetMap PBF file format.
* [osm_boundaries_utils_rs](https://github.com/Qwant/osm_boundaries_utils_rs) - Read OpenStretMap relations with type=boundary as valid MultiPolygon.
* [osm-transit-extractor](https://github.com/CanalTP/osm-transit-extractor) - Extract OSM public transport data and write to CSV files.
* [Pbfextractor](https://github.com/Lesstat/pbfextractor) - Create graph files out of OSM and SRTM data
* [osmflat](https://github.com/boxdot/osmflat-rs) - OpenStreetMap flatdata format and compiler.

More crates based on [osmpbfreader-rs](https://crates.io/crates/osmpbfreader/reverse_dependencies)

### 3D
* [density mesh](https://github.com/PsichiX/density-mesh) - Image density/height map to mesh generator.
* [startin](https://github.com/hugoledoux/startin) - A Delaunay triangulator for processing TINs.

### Geocoding
* [GeoHash](https://github.com/georust/geohash) - Compute geohash of locations.
* [Geocoding](https://github.com/georust/geocoding) - Enrich addresses, cities, countries with geographic coordinates through third-party geocoding web services.
* [Mimirsbrunn](https://github.com/CanalTP/mimirsbrunn) - Geocoding and reverse-geocoding (with OSM data).

### Routing
* [Fast Paths](https://github.com/easbar/fast_paths) - Fast shortest path calculations for Rust.
* [osm_ch](https://github.com/Stunkymonkey/osm_ch) - OSM-Contraction-Hierarchies.

### Web Services
* [t-rex](https://t-rex.tileserver.ch/) - Vector tile server specialized on publishing MVT tiles from your own data.
* [Martin](https://github.com/urbica/martin) - Blazing fast and lightweight PostGIS vector tiles server.
* [Hecate](https://github.com/mapbox/Hecate) - Fast Geospatial Feature Storage API.

### Map rendering
* [osm-renderer](https://github.com/dfyz/osm-renderer) - OpenStreetMap raster tile renderer.

### Applications
* [A/B Street](https://github.com/a-b-street/abstreet) - A traffic simulation game exploring how small changes to roads affect cyclists, transit users, pedestrians, and drivers.
* [Geo Engine](https://github.com/geo-engine/geoengine) - Cloud-ready geospatial data processing platform with workflows, raster *and* vector support and OGC-compliant interfaces.
* [sst](https://github.com/hugoledoux/sst) - streaming startin.
* [WhiteboxTools](https://github.com/jblindsay/whitebox-tools) - Geospatial data analysis platform with more than 465 tools for processing various types of geospatial data. 

## Watchlist

* [Rust Geodesy](https://github.com/busstoptaktik/geodesy/) - A platform for experiments with geodetic software, transformations, and standards.
* [coord_transforms](https://github.com/DaveKram/coord_transforms) - Rust crate for performing coordinate transforms.
* [maplibre-rs](https://github.com/maplibre/maplibre-rs/) - Native Maps for Web, Mobile and Desktop.
* [RGeometry](https://github.com/rgeometry/rgeometry) - Computational Geometry library written in Rust.
* [offset-polygon](https://github.com/anlumo/offset_polygon) - A Rust crate for offsetting (shrinking/expanding) polygons.
* [map-engine](https://gitlab.com/spadarian/map-engine/) - A rust library to work with tiled geospatial (raster) data.
* [rgis](https://github.com/frewsxcv/rgis) - Geospatial data viewer (web and desktop).
* [rust_road_router](https://github.com/kit-algo/rust_road_router) - Rust routing framework and toolkit.
* [Sailor](https://github.com/Yatekii/sailor) - A sailing navigation application.
* [OGC API](https://github.com/camptocamp/ogcapi) - OGC API building blocks.
* [copc-rs](https://github.com/pka/copc-rs) - COPC reader.

## Resources

### Community
* [Discord](https://discord.gg/Fp2aape) - GeoRust Discord channel
