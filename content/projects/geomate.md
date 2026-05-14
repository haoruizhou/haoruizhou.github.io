### GEOMATE XODR PIPELINE
**GeoMate Inc. | Python / AWS / Terraform / OSM / XODR**

End-to-end geospatial data engineering pipeline for autonomous driving simulation. Procedurally generates valid OpenDRIVE (XODR) road networks from raw multi-source geospatial data — not format conversion, but full procedural generation.

### Technical Challenge
- Input: raw OpenStreetMap node/way topology, Overture Maps, DEM elevation data
- Output: drivable, topologically correct XODR XML validated in the CARLA autonomous driving simulator
- Core problem: stitching OSM node/way topology into the lane-centric road model XODR requires — resolving junctions, inferring lane geometry, ensuring topological correctness

### Infrastructure
- AWS stack: S3, EC2, ECS, Lambda, Fargate, RDS
- Terraform IaC for reproducible, scalable infrastructure provisioning
- Self-hosted OSM infrastructure (SliceOSM / Overpass-style) for custom extract pipelines
- Pytest-based automated data validation and QA pipelines

### Also Owns
- Commercial OD data → SUMO traffic simulation pipeline
- Spatial data lake architecture supporting high-volume geospatial processing
