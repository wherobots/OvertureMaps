# Harnessing Overture Maps Data: Apache Sedona’s Journey from Parquet to GeoParquet

This repo provides the notebooks used in the Wherobots blogpost: https://medium.com/@dr.jiayu/harnessing-overture-maps-data-apache-sedonas-journey-from-parquet-to-geoparquet-d99f7767a499

* [Study 1](https://github.com/wherobots/OvertureMaps/blob/main/Sedona_OvertureMaps_Parquet.ipynb): Analyze the OMF Parquet data using Sedona
* [Study 2](https://github.com/wherobots/OvertureMaps/blob/main/Sedona_OvertureMaps_Parquet_To_GeoParquet.ipynb): Converting from Parquet to GeoParquet
* [Study 3](https://github.com/wherobots/OvertureMaps/blob/main/Sedona_OvertureMaps_GeoParquet.ipynb): Interactive geospatial spatial analytics on OMF GeoParquet data

## Interactive notebook using GeoParquet and Sedona

- The interactive notebook used in Study 3 is packaged in the official Apache Sedona Docker image: https://hub.docker.com/r/apache/sedona
- Pull the Docker image: You can do `docker pull apache/sedona` and then run `docker run -p 8888:8888 apache/sedona:latest`
- Start coding: The Jupyter notebook will be available at https://localhost:8888

## Use Wherobots Cloud to easily run Sedona

The other notebooks used in Study 1 and 2 can be run on Wherobots cloud with a [professional plan](https://wherobots.com/pricing/). If you want to try them out, please sign up to [Wherobots Cloud](https://wherobots.services/) and [contact us](https://docs.wherobots.services/latest/support/) to upgrade.

Wherobots is the spatial analytics and AI cloud, trusted in production, at scale, from the original creators of Apache Sedona.

## Free and public Overture Maps GeoParquet data from Wherobots

The GeoParquet format data produced in Study 2 is provided by [Wherobots](https://www.wherobots.ai/) for free. It has the same schema and license as the original Overture Maps Parquet data, except the geometry column is in `geometry` type and has additional `geohash` column in string type. You can access them as follows:

- Buildings: `s3://wherobots-examples/data/overturemaps-us-west-2/release/2023-07-26-alpha.0/theme=buildings/type=building`
- Places: `s3://wherobots-examples/data/overturemaps-us-west-2/release/2023-07-26-alpha.0/theme=places/type=place`
- AdminBoundary: `s3://wherobots-examples/data/overturemaps-us-west-2/release/2023-07-26-alpha.0/theme=admins/type=administrativeBoundary`
- AdminLocality: `s3://wherobots-examples/data/overturemaps-us-west-2/release/2023-07-26-alpha.0/theme=admins/type=locality`
- Transportation Connector: `s3://wherobots-examples/data/overturemaps-us-west-2/release/2023-07-26-alpha.0/theme=transportation/type=connector`
- Transportation Segment: `s3://wherobots-examples/data/overturemaps-us-west-2/release/2023-07-26-alpha.0/theme=transportation/type=segment`

## Licenses

The licenses of the Wherobots Overture Maps data are the same as the [original Overture Map data licenses](https://overturemaps.org/download/).

## Credits

Furqaan Khan, Jia Yu, Mo Sarwat, Nilesh Gajwani, Kristin Cowalcijk
