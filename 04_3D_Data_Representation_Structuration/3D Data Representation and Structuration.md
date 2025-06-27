3D Data Representation -- point clouds, meshes, parametric models, voxels, and depth maps (various ways to describe and handle 3D geometric entities)

![[Pasted image 20250627132525.png]]

**3D Point Clouds:**
- comprises of a set of data points -- usually expressed in a 3D coordinate system (x, y, z)

(main operations)
- Transformations: You can multiply the points in the point list with linear transformation matrices
- Combinations: Objects can be combined by merging the point list
- Rendering: Projects and draws the points onto an image plane
(main benefits)
- Fast rendering
- Exact representation
- Fast transformations
(main disadvantages)
- Numerous points (object curve, exact representation)
- High memory consumption
- Limited combination operations

(common point cloud file format)
.ply (polygon file format) - open3d, pyvista 
(simple, versatile, great for prototyping, human readability is a plus, can handle various attributes)

.las/.laz (LAS/LAZ formats) - laspy
(indutry standard for LiDAR, .laz offers significant compression benefits for large datasets - essential for efficient storage and processing)

.xyz (Simple text file) - pandas, numpy
(barebone format often used for basic point coordinates (x, y, z), lacks metadata capabilities)

.pts (Leica point cloud format) - pdal, open3d
(commonly used in surveying and CAD, versatile, sometimes requires tailored parsing due to its proprietary nature)

.e57 (ASTM E57 3D Imaging Data Exchange Format) - pye57, e57, pdal
(emerging standard designed for interoperability, handles rich metadata and point attributes, crucial for complex 3D projects)

.obj (Wavefront OBJ) - open3d, pywavefront
(more focused on mesh data but can represent point clouds, commonly used in computer graphics and 3D modelling, often paired with .mtl files for material definitions)

.pcd (Point Cloud Data file format) - open3d, pcl, pyntcloud
(preferred format for the Point Cloud Library (PCL), commonly used in robotics and computer vision research)

**Image-based Representations:**
(How can we tie 3D representations to 2D images?)

Depth maps:
- raster images -- main image channel provides depth-based separation between pixels that make up a scene, as seen from one particular perspective
- color-coding intensity values on one channel are the simplest way to convey depth
- bright pixels have the highest value, and dark pixel have the lowest value
- depth image -- presents values according to the objects' distance
- pixel color -- gives the distance from the camera
- depth map is related to the z-buffer (z relates to the direction of a camera's central axis of view, not the absolute z scene coordinate)

(operations)
- Transformations: Multiply the pixels in the image with linear transformation matrices
- Combinations: Objects can be combined by merging the point lists
- Rendering: Draws pixels on the image plane

(benefits)
- Low memory requirements
- Very well-known raster format
- Transformations are quick and easy

(disadvantages)
- essentially, a 2.5D representation
- cannot describe a whole 3D scene on its own
- weak topology

Can extend depth maps to a particular case called RGB-D (RGB-D data provides 2.5D information about the captured 3D object by attaching the depth map and 2D color information (RGB))

Projections:
To display raw 3D data is to project it onto a different 2D space, capturing some of the essential characteristics of the original 3D shape.

