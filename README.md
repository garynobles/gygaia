# gygaia
This project is a workflow to take photogrametry of archaeological contexts and create volumetric entities.

Docker
Install docker, best to use windows 10

PDAL





docker run -it --rm -v /p/KAP:/opt/data chambbj/pdal-noble-kernel pdal noble /opt/data/1.las /opt/data/2.las /opt/data/out1_2_1cm.las 0.01

#create a polygon of common area to clip against the resulting pointcloud or original pointcloud
// these commands calculte the bounds of the pointcloud.
docker run -it --rm -v /p/KAP:/opt/data chambbj/pdal-noble-kernel pdal info opt/data/1.las --boundary
docker run -it --rm -v /p/KAP:/opt/data chambbj/pdal-noble-kernel pdal info opt/data/2.las --boundary

#combine


// clip each pointcloud so they have the same bounding area.



// create a clean pointcloud with top and base



// store the pointclods in a postgresql db so the above can be achieved progametically

// store the created volume pointclouds in the db

// use Postgresql to create solid volumes ready for 3D queries

// test selecting objects in volumes

// export volumes as STL for 3D printing
