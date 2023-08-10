# Free and Ready-to-use OvertureMaps GeoParquet data provided by Wherobots

Wherobots provides ready to use spatially-indexed / sorted Overture Maps Data for free

This repo provides the notebooks used in the Wherobots blogpost.

## Interactive notebook using GeoParquet and Sedona

- The interactive notebook used in Study 3 is packaged in the official Apache Sedona Docker image: https://hub.docker.com/r/apache/sedona
- Pull the Docker image: You can do `docker pull apache/sedona` and then run `docker run -p 8888:8888 apache/sedona:latest`
- Start coding: The Jupyter notebook will be available at https://localhost:8888

## Use Wherobots to deploy Sedona to cloud vendors

The other notebooks used in Study 1 and 2 can be run on a AWS EMR or Databricks cluster. if you want to try them out, please sign up here: https://www.wherobots.ai/demo

## Free and public Overture Maps GeoParquet data from Wherobots

The GeoParquet format data produced in Study 2 is provided by [Wherobots](https://www.wherobots.ai/) for free. It has the same schema and license as the original Overture Maps Parquet data, except the geometry column is in `geometry` type and has additional `geohash` column in string type. You can access them as follows:

- Buildings: `s3://wherobots-public-data/overturemaps-us-west-2/release/2023-07-26-alpha.0/theme=buildings/type=building`
- Places: `s3://wherobots-public-data/overturemaps-us-west-2/release/2023-07-26-alpha.0/theme=places/type=place`
- AdminBoundary: `s3://wherobots-public-data/overturemaps-us-west-2/release/2023-07-26-alpha.0/theme=admins/type=administrativeBoundary`
- AdminLocality: `s3://wherobots-public-data/overturemaps-us-west-2/release/2023-07-26-alpha.0/theme=admins/type=locality`
- Transportation Connector: `s3://wherobots-public-data/overturemaps-us-west-2/release/2023-07-26-alpha.0/theme=transportation/type=connector`
- Transportation Segment: `s3://wherobots-public-data/overturemaps-us-west-2/release/2023-07-26-alpha.0/theme=transportation/type=segment`

## Licenses

The licenses of the Wherobots Overture Maps data are the same as the [original Overture Map data licenses](https://overturemaps.org/download/).