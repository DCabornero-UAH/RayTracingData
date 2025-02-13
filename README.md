This is a data repository with all the geometries included in the paper "Acceleration of Deterministic Ray Tracing with PostgreSQL and PostGIS."

Two experiments have been performed on this paper:
 
- A comparison between a Fortran implementation and the PostGIS implementation. Six geometries have been used, and they can be found in STL format in the meshes folder.
- A performance study of the Cassegrain reflector that was only performed with PostGIS. The whole set of meshes created with the same object and meshed with a distinct number of facets can be found in STL format in the *cassegrain_reflector* folder.

Apart from this, the *observation_points* folder provides *txt* files with the location of the 2500 observation points used on each experiment.

Each source point of light is indicated in the following table:

| **Geometry**         | **Source point** |
|----------------------|------------------|
| 2 plates             | (0,0,1)          |
| 3 plates             | (0,0,1)          |
| Park                 | (2,0,4.3)        |
| Turbine              | (-30,-30,2)      |
| Paraboloid           | (0,0,1)          |
| Paraboloid and plate | (0,0,1)          |

Besides, these geometries can be rebuilt with this information:

| **Geometry**         | **Source point**                                                                                              |
|----------------------|---------------------------------------------------------------------------------------------------------------|
| 2 plates             | The plates are built from (0,0,z) to (5,5,z)<br>There are two plates: one at z=0 and one at z=5               |
| 3 plates             | The plates are built from (0,0,z) to (5,5,z)<br>There are two plates: one at z=0, one at z=2.5 and one at z=5 |
| Paraboloid           | Center: (0,0,0)<br>Focal distance: 2<br>Radius: 2                                                             |
| Paraboloid and plate | Center: (0,0,0)<br>Diameter: 5<br>Focal length: 2.5<br>Height: 2<br>Feed: 0.5      