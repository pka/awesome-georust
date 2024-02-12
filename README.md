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
    - [Spatial index / Partioning](#spatial-index--partioning)
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
* [Rust Geodesy](https://github.com/busstoptaktik/geodesy/) - A geodesy library written in Rust.
* [geographiclib-rs](https://github.com/georust/geographiclib-rs) - A port of geographiclib (geodesic calculations).
* [S2](https://github.com/danhhz/s2) - S2 spherical geometry library in Rust.
* [rust-geo-booleanop](https://github.com/21re/rust-geo-booleanop) - Rust implementation of the Martinez-Rueda Polygon Clipping Algorithm.
* [intersect2d](https://github.com/eadf/intersect2d.rs) - Line intersection sweep-line algorithm.
* [spatial-join](https://github.com/msalib/spatial-join) - Perform streaming geospatial-joins on geographic data.
* [tile-grid](https://crates.io/crates/tile-grid) - Library for map tile grid calculations.
* [zonebuilder](https://github.com/zonebuilders/zonebuilder-rust) - Build zones for large geographic regions.
* [Polylabel-rs](https://github.com/urschrei/polylabel-rs) - A Rust implementation of the Polylabel algorithm, with FFI.
* [cheap-ruler-rs](https://github.com/vipera/cheap-ruler-rs) - Collection of very fast approximations to common geodesic measurements.

### Spatial index / Partioning
* [rstar](https://github.com/georust/rstar) - R\*-tree library for the rust ecosystem.
* [kdbush](https://github.com/pka/rust-kdbush) - A Rust port of kdbush, a fast static spatial index for 2D points.
* [spade](https://github.com/Stoeoef/spade) - Delaunay Triangulations for the Rust ecosystem.
* [delaunator-rs](https://github.com/mourner/delaunator-rs) - A very fast static 2D Delaunay triangulation library for Rust.
* [earcutr](https://github.com/frewsxcv/earcutr) - Port of MapBox's earcut triangulation code to Rust language.
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
* [RINEX](https://github.com/georust/rinex) - RINEX analysis & and processing.
* [shapefile-rs](https://github.com/tmontaigu/shapefile-rs) - Rust library to read & write shapefiles.
* [TileJSON](https://github.com/georust/tilejson) - Work with TileJSON files.
* [Transit](https://github.com/georust/transitfeed) - Work with GTFS files.
* [transit_model](https://github.com/hove-io/transit_model) - Manage, convert and enrich transit data.
* [FastGtfs](https://github.com/nicomazz/fastgtfs) - GTFS parsing, navigation, time table creation, and real-time network simulation.
* [gtfs-structures](https://github.com/rust-transit/gtfs-structure) - Read GTFS files into structs, with smart references.
* [WKT](https://github.com/georust/wkt) - Work with Well-Known Text (WKT) files.
* [World file](https://github.com/georust/world-file) - Work with World-files.
* [FlatGeobuf](https://github.com/flatgeobuf/flatgeobuf) - A performant binary encoding for geographic data based on flatbuffers.
* [las-rs](https://github.com/gadomski/las-rs) - Read and write ASPRS las files.
* [stac-rs](https://github.com/gadomski/stac-rs) - Rust implementation of the SpatioTemporal Asset Catalog (STAC) specification.
* [pgstac-rs](https://github.com/gadomski/pgstac-rs) - Rust interface for [pgstac](https://github.com/stac-utils/pgstac).

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
* [osm-lump-ways](https://github.com/amandasaurus/osm-lump-ways) - Group OSM ways based on topology & shared tags

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
* [Martin](https://github.com/maplibre/martin) - Blazing fast and lightweight PostGIS vector tiles server.
* [Hecate](https://github.com/mapbox/Hecate) - Fast Geospatial Feature Storage API.

### Map rendering
* [osm-renderer](https://github.com/dfyz/osm-renderer) - OpenStreetMap raster tile renderer.

### Applications
* [A/B Street](https://github.com/a-b-street/abstreet) - A traffic simulation game exploring how small changes to roads affect cyclists, transit users, pedestrians, and drivers.
* [Geo Engine](https://github.com/geo-engine/geoengine) - Cloud-ready geospatial data processing platform with workflows, raster *and* vector support and OGC-compliant interfaces.
* [rgis](https://github.com/frewsxcv/rgis) - Performant, cross-platform (web, desktop) GIS app written in Rust 
* [sst](https://github.com/hugoledoux/sst) - streaming startin.
* [WhiteboxTools](https://github.com/jblindsay/whitebox-tools) - Geospatial data analysis platform with more than 465 tools for processing various types of geospatial data. 

## Watchlist

* [Miniproj](https://git.geomar.de/flemming-staebler/miniproj) - Geographic transformations between different coordinate systems defined by the European Petroleum Survey Group.
* [coord_transforms](https://github.com/DaveKram/coord_transforms) - Rust crate for performing coordinate transforms.
* [maplibre-rs](https://github.com/maplibre/maplibre-rs/) - Native Maps for Web, Mobile and Desktop.
* [RGeometry](https://github.com/rgeometry/rgeometry) - Computational Geometry library written in Rust.
* [offset-polygon](https://github.com/anlumo/offset_polygon) - A Rust crate for offsetting (shrinking/expanding) polygons.
* [map-engine](https://gitlab.com/spadarian/map-engine/) - A rust library to work with tiled geospatial (raster) data.
* [rust_road_router](https://github.com/kit-algo/rust_road_router) - Rust routing framework and toolkit.
* [Sailor](https://github.com/Yatekii/sailor) - A sailing navigation application.
* [OGC API](https://github.com/georust/ogcapi) - OGC API building blocks.
* [copc-rs](https://github.com/pka/copc-rs) - COPC reader.
* [zarrs](https://github.com/LDeakin/zarrs) - A rust library for the Zarr V3 storage format for multidimensional arrays and metadata.
* [pasture](https://github.com/Mortano/pasture) - A Rust library for working with point cloud data.
* [h3o](https://github.com/HydroniumLabs/h3o) - Rust implementation of the H3 geospatial indexing system.
* [bevy-potree](https://github.com/ForesightMiningSoftwareCorporation/bevy-potree)
* [cogbuilder](https://github.com/fintelia/cogbuilder)
* [vrt-file](https://github.com/fintelia/vrt-file)
* [PlanetVectorTile](https://github.com/planet-vector-tile/planet-vector-tile) - A map engine enabling you to have the entire map of the OSM planet on your own computer.
* [GeoPolars](https://github.com/geopolars/geopolars) - Geospatial extensions for Polars.
* [country-geocoder](https://github.com/a-b-street/country-geocoder) - Reverse geocode WGS84 coordinates to an ISO country-code.
* [Skeleton Tracing](https://github.com/LingDong-/skeleton-tracing/tree/master/rs) - A new algorithm for retrieving topological skeleton as a set of polylines from binary images.
* [poly2tri-rs](https://github.com/shuoli84/poly2tri-rs) - Calculate CDT (Constrained Delaunay Triangulation) on a polygon.
* [PMTiles (for Rust)](https://github.com/stadiamaps/pmtiles-rs) - Rust implementation of PMTiles
* [PMTiles (for Rust)](https://github.com/arma-place/pmtiles-rs) - Low level implementation of the PMTiles format
* [Proj4rs](https://github.com/3liz/proj4rs) - Rust adaptation of Proj4
* [Proj4wkt](https://github.com/3liz/proj4wkt-rs) - Parse WKT to Proj strings 
* [Louvre](https://github.com/acheul/louvre) - Computational Geometry Library with Rust
* [gpkg-rs](https://github.com/cjriley9/gpkg-rs) - A Rust crate for reading and writing GeoPackages.
* [georaster](https://github.com/pka/georaster) - Rust library for accessing geospatial raster images (GeoTIFF).

## Resources

### crates.io
* Category [Science::Geospatial](https://crates.io/categories/science::geo)

### Community
* [Discord](https://discord.gg/Fp2aape) - GeoRust Discord channel
