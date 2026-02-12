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
* [flat-projection](https://github.com/Turbo87/flat-projection-rs) - Fast geodesic distance approximations via flat surface projection.
* [sguaba](https://github.com/helsing-ai/sguaba) - Types for points and vectors in coordinate spaces and transformations based on rigid body transforms.
* [geocentric-rs](https://github.com/ciscorn/geocentric-rs) - Conversion between geodetic (geographic) and geocentric (cartesian) coordinates.

### Spatial index / Partioning
* [rstar](https://github.com/georust/rstar) - R\*-tree library for the rust ecosystem.
* [kdtree](https://github.com/mrhooray/kdtree-rs) - K-dimensional tree in Rust for fast geospatial indexing and nearest neighbors lookup
* [sif-rtree](https://github.com/adamreichold/sif-rtree) and [sif-kdtree](https://github.com/adamreichold/sif-kdtree) - R and K-D trees which can be memory-mapped directly from disk.
* [geo-index](https://github.com/kylebarron/geo-index) - Fast, immutable, ABI-stable spatial indexes.
* [kdbush](https://github.com/pka/rust-kdbush) - A Rust port of kdbush, a fast static spatial index for 2D points.
* [static-bushes](https://github.com/apendleton/static-bushes) - Port of the Flatbush and KDBush JS libraries to Rust.
* [spade](https://github.com/Stoeoef/spade) - Delaunay Triangulations for the Rust ecosystem.
* [delaunator-rs](https://github.com/mourner/delaunator-rs) - A very fast static 2D Delaunay triangulation library for Rust.
3 [Delatin](https://github.com/pokhanto/delatin-rs) - Simple and fast TIN generation library,
* [earcutr](https://github.com/frewsxcv/earcutr) - Port of MapBox's earcut triangulation code to Rust language.
* [iTriangle](https://github.com/iShape-Rust/iTriangle) - A fast, stable, and robust 2d triangulation library.
* [boostvoronoi](https://github.com/eadf/boostvoronoi.rs) - Segmented Voronoi for Rust.
* [geo-quadkey-rs](https://github.com/masaishi/geo-quadkey-rs) - Rust library for encoding and decoding geographical coordinates to and from QuadKeys.
* [h3o](https://github.com/HydroniumLabs/h3o) - Rust implementation of the H3 geospatial indexing system.
* [Quadbin](https://github.com/atsyplenkov/qbin) - Hierarchical geospatial index tiling, similar to Quadkey.
* [A5](https://a5geo.org/docs/quickstart/rust) - Rust library for the A5 geospatial indexing system, a new alternative to S2 and H3 using irregular, equilateral pentagons.

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
* [cql2-rs](https://github.com/developmentseed/cql2-rs) - Library for parsing the OGC CQL2 filter language.

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
* [osmx](https://github.com/jake-low/osmx-rs) - Rust port of OSMExpress, a fast database file format for OpenStreetMap.
* [osm-lump-ways](https://github.com/amandasaurus/osm-lump-ways) - Group OSM ways based on topology & shared tags
* [osm-pbf-parquet](https://github.com/OvertureMaps/osm-pbf-parquet) - Transcode OSM PBF file to parquet files.

More crates based on [osmpbfreader-rs](https://crates.io/crates/osmpbfreader/reverse_dependencies)

### 3D
* [density mesh](https://github.com/PsichiX/density-mesh) - Image density/height map to mesh generator.
* [startin](https://github.com/hugoledoux/startin) - A Delaunay triangulator for processing TINs.
* [geom3d](https://github.com/J-F-Liu/geom3d) - Data structures and algorithms for 3D geometric modeling.

### Geocoding
* [GeoHash](https://github.com/georust/geohash) - Compute geohash of locations.
* [Geocoding](https://github.com/georust/geocoding) - Enrich addresses, cities, countries with geographic coordinates through third-party geocoding web services.
* [Airmail](https://github.com/ellenhp/airmail) - Lightweight geocoder in pure Rust.
* [country-boundaries](https://github.com/westnordost/country-boundaries-rust) - A fast offline reverse geocoder: Find the area in which a geo position is located.

### Routing
* [Fast Paths](https://github.com/easbar/fast_paths) - Fast shortest path calculations for Rust.
* [osm_ch](https://github.com/Stunkymonkey/osm_ch) - OSM-Contraction-Hierarchies.
* [routrs](https://github.com/routrs/routrs) - Geograph-based shortest distance calculation for Rust.
* [rustworkx](https://github.com/Qiskit/rustworkx) - A high-performance, general-purpose graph library for Python, written in Rust.
* [RouteE Compass](https://github.com/NREL/routee-compass) - An energy-aware vehicle routing engine.
* [Routers](https://github.com/routers-org/routers) - Set of routing tools designed for system-agnostic maps.

### Web Services
* [t-rex](https://github.com/t-rex-tileserver/t-rex) - Vector tile server specialized on publishing MVT tiles from your own data.
* [Martin](https://github.com/maplibre/martin) - Blazing fast and lightweight PostGIS, MBtiles and PMtiles tile server with support for tile generation and mbtiles tooling.
* [Hecate](https://github.com/mapbox/Hecate) - Fast Geospatial Feature Storage API.
* [BBOX services](https://github.com/bbox-services/bbox) - Composable spatial services.
* [MVT Server](https://github.com/mvt-proj/mvt-rs) - Simple and high-speed vector tile server with a built-in web-based admin interface.

### Map rendering
* [osm-renderer](https://github.com/dfyz/osm-renderer) - OpenStreetMap raster tile renderer.

### Applications
* [A/B Street](https://github.com/a-b-street/abstreet) - A traffic simulation game exploring how small changes to roads affect cyclists, transit users, pedestrians, and drivers.
* [Geo Engine](https://github.com/geo-engine/geoengine) - Cloud-ready geospatial data processing platform with workflows, raster *and* vector support and OGC-compliant interfaces.
* [rgis](https://github.com/frewsxcv/rgis) - Performant, cross-platform (web, desktop) GIS app written in Rust
* [sst](https://github.com/hugoledoux/sst) - streaming startin.
* [WhiteboxTools](https://github.com/jblindsay/whitebox-tools) - Geospatial data analysis platform with more than 465 tools for processing various types of geospatial data.
* [Ferrostar](https://github.com/stadiamaps/ferrostar) - A FOSS navigation SDK built from the ground up for the future.
* [Arnis](https://github.com/louis-e/arnis) - Generate any location from the real world in Minecraft Java Edition with a high level of detail.
* [Karttapullautin](https://github.com/karttapullautin/karttapullautin) - A fast and accurate map generator from classified LiDAR data.
* [SedonaDB](https://github.com/apache/sedona-db) - Single-node analytical database engine with geospatial as the first-class citizen.
* [Vector Tile Builder](https://github.com/ShogoHirasawa/web-vector-tile-maker) - Web application for generating vector tiles in the browser

## Watchlist

* [Miniproj](https://git.geomar.de/flemming-staebler/miniproj) - Geographic transformations between different coordinate systems defined by the European Petroleum Survey Group.
* [coord_transforms](https://github.com/DaveKram/coord_transforms) - Rust crate for performing coordinate transforms.
* [maplibre-rs](https://github.com/maplibre/maplibre-rs/) - Native Maps for Web, Mobile and Desktop.
* [RGeometry](https://github.com/rgeometry/rgeometry) - Computational Geometry library written in Rust.
* [offset-polygon](https://github.com/anlumo/offset_polygon) - A Rust crate for offsetting (shrinking/expanding) polygons.
* [polygon-offsetting](https://github.com/Akirami/polygon-offsetting) - Offset a polygon (only margin).
* [Cavalier Contours](https://github.com/jbuckmccready/cavalier_contours) - 2D polyline/shape library for offsetting, combining, etc.
* [map-engine](https://gitlab.com/spadarian/map-engine/) - A rust library to work with tiled geospatial (raster) data.
* [rust_road_router](https://github.com/kit-algo/rust_road_router) - Rust routing framework and toolkit.
* [Sailor](https://github.com/Yatekii/sailor) - A sailing navigation application.
* [OGC API](https://github.com/georust/ogcapi) - OGC API building blocks.
* [copc-rs](https://github.com/pka/copc-rs) - Cloud Optimized Point Cloud (COPC) reader and writer.
* [zarrs](https://github.com/LDeakin/zarrs) - A rust library for the Zarr V3 storage format for multidimensional arrays and metadata.
* [pasture](https://github.com/Mortano/pasture) - A Rust library for working with point cloud data.
* [bevy-potree](https://github.com/ForesightMiningSoftwareCorporation/bevy-potree)
* [cogbuilder](https://github.com/fintelia/cogbuilder)
* [vrt-file](https://github.com/fintelia/vrt-file)
* [PlanetVectorTile](https://github.com/planet-vector-tile/planet-vector-tile) - A map engine enabling you to have the entire map of the OSM planet on your own computer.
* [GeoPolars](https://github.com/geopolars/geopolars) - Geospatial extensions for Polars.
* [Polars ST](https://github.com/Oreilles/polars-st) - Spatial extension for Polars DataFrames.
* [Skeleton Tracing](https://github.com/LingDong-/skeleton-tracing/tree/master/rs) - A new algorithm for retrieving topological skeleton as a set of polylines from binary images.
* [poly2tri-rs](https://github.com/shuoli84/poly2tri-rs) - Calculate CDT (Constrained Delaunay Triangulation) on a polygon.
* [PMTiles (for Rust)](https://github.com/stadiamaps/pmtiles-rs) - Rust implementation of PMTiles
* [PMTiles (for Rust)](https://github.com/arma-place/pmtiles-rs) - Low level implementation of the PMTiles format
* [s2-pmtiles](https://github.com/Open-S2/s2-pmtiles) - Read/Write PMTiles V3.0 as well as S2PMTiles V1.0
* [Proj4rs](https://github.com/3liz/proj4rs) - Rust adaptation of Proj4
* [Proj4wkt](https://github.com/3liz/proj4wkt-rs) - Parse WKT to Proj strings
* [Louvre](https://github.com/acheul/louvre) - Computational Geometry Library with Rust
* [gpkg-rs](https://github.com/cjriley9/gpkg-rs) - A Rust crate for reading and writing GeoPackages.
* [georaster](https://github.com/pka/georaster) - Rust library for accessing geospatial raster images (GeoTIFF).
* [jord](https://github.com/ofmooseandmen/jord-rs) - Geographical Position Calculations (spherical + ellipsoidal models and local frames).
* [tzf-rs](https://github.com/ringsaturn/tzf-rs) - Get timezone via longitude&latitude in Rust in a fast way
* [geometry-rs](https://github.com/ringsaturn/geometry-rs) - Partial port of tidwall/geometry (efficient 2D geometry library for Go).
* [pasture](https://github.com/Mortano/pasture) - Rust library for point cloud processing.
* [rout3serv](https://github.com/nmandery/rout3serv) - H3-grid based Routing server with GRPC-API and dataframe integration.
* [geoserde](https://github.com/p4ken/geoserde) - Adapter between geographic feature and GIS files.
* [geojson-vt-rs](https://github.com/maxammann/geojson-vt-rs) - Crate for slicing GeoJSON into vector tiles on the fly.
* [The Roaring Landmask](https://github.com/gauteh/roaring-landmask) - A fast and memory-limited landmask based on GSHHG for determing whether a point on Earth is on land or in the ocean.
* [Galileo](https://github.com/Maximkaaa/galileo) - General purpose cross-platform geo-rendering library.
* [Gauzilla](https://github.com/BladeTransformerLLC/gauzilla) - 3D Gaussian Splatting renderer for WebAssembly with lock-free multithreading.
* [utiles](https://github.com/jessekrubin/utiles) - utils & tiles w/ (rs & pyo3).
* [earclip](https://github.com/Open-S2/earclip) - Triangle mesh designed to be fast, efficient, and sphere capable.
* [iOverlay](https://github.com/iShape-Rust/iOverlay) - Boolean Operations for 2D Polygons: Supports intersection, union, difference, xor, and self-intersections for all polygon varieties.
* [linesweeper](https://github.com/jneem/linesweeper) - Two-dimensional geometric primitives like boolean operations on sets bounded by Bézier paths.
* [Solari](https://github.com/ellenhp/solari) - Multimodal routing in Rust.
* [plateau-gis-converter](https://github.com/MIERUNE/plateau-gis-converter) - A GUI and CLI tool for converting PLATEAU's 3D city models (CityGML) of Japan into various geospatial formats, including 3D Tiles, MVT, and GeoPackage.
* [anime](https://github.com/JosiahParry/anime) - Approximate Network Matching, Integration, and Enrichment.
* [rusterize](https://github.com/ttrotto/rusterize) - High performance rasterization tool for python built in Rust.
* [maplibre-legend](https://github.com/mvt-proj/maplibre-legend) - Maplibre legend generator crate.
* [geocart](https://github.com/HectorMRC/geocart) - A bridge between geographic and cartesian coordinates.
* [Bevy Point Cloud](https://github.com/rlamarche/bevy_pointcloud) - A Bevy plugin to render point clouds.
* [CGAR](https://github.com/aseverino/cgar) - Computational Geometry Algorithms for Rust.
* [etiles](https://github.com/tum-gis/etiles) - A Rust library for processing 3D Tiles data.
* [rusqlite-gpkg](https://github.com/yutannihilation/rusqlite-gpkg) - GeoPackage reader/writer built on top of rusqlite.


## Resources

### crates.io
* Category [Science::Geospatial](https://crates.io/categories/science::geo)

### Community
* [Discord](https://discord.gg/Fp2aape) - GeoRust Discord channel
