The four core components of 3D data science:
1. 3D data science and spatial AI concepts
2. 3D data: fundamental building blocks
3. The modular 3D workflow
4. 3D data science in the industry

This filed bridges the gap between our 3D world and the science of extracting knowledge and insights from data. 

Dimensions and 3D data Science:
dimension -- a measurable aspect or characteristics of something
(from mathematical point of view) dimension -- refers to the number of variables needed to describe a system or object. 
(from 4D data science perspective) dimension -- refers to spatial extent

1D object -- describe by a single variable
2D data -- two dimensions, typically with x and y coordinates
3D data -- points in space defined by x, y, and z coordinates
(a chair is a 3D object because it has length, width, and height, allowing us to distinguish it from a picture of a chair, which is a 2D representation)

Spatial AI -- powerful tool that allow a machines to perceive, reason about, and interact with the world in a way that mimics human spatial intelligence. 
(similar to giving computers a pair of eyes that can see beyond the flat screen, understanding the nuances of depth, distance, and orientation)
It is comprised of foundational components including:
1. Perception -- how do machines see the world in 3D (sensors like LiDAR, cameras, and depth sensors capture spatial information)
2. Reasoning -- once machines have perceived the world, how do they make sense of it (algorithms and techniques enable spatial reasoning and decision making)
3. Action -- how can machines translate their understanding of the 3D world into meaningful actions (accurate digital environments form a robust base)

![[Pasted image 20250624231315.png]]

The fusion process permits the linking of the data from the sensor in the real world, which can be fed back into the digital twin. The simulations or models can be updated to reflect the changing conditions in the real world. This creates a feedback loop between the two worlds.

3D Data: Fundamental Building Blocks
primary objective of 3D data science -- to define the boundaries of a 'digital environment'

we want to create a replica of the world we inhabit -- this will serve as a robust foundation for our digital applications -- precise digital representation of the real world will then enable intelligent agents to perform tasks in a manner that resembles human behaviour -- once the foundations are established, we can connect to decision-making elements that can be triggered through voice commands, manipulations, or other means. 

real world (as our base) -- take the base to create a low-level digital model (geometric depiction of what we observe) -- create a high-level digital model (used for reasoning services)

3D data science workflow, which relies on point cloud datasets -- usually application specific
(follows a classical progression from gathering relevant data to creating deliverables)

![[Pasted image 20250624232902.png]]

![[Pasted image 20250624233013.png]]
High-level view of the 3D data science workflow

Data Acquisition -- we rely essentially (but not only) on 3D sensors that allow us to capture the 3D shape and sometimes even other properties of objects and scenes. 
Pre-processing
![[Pasted image 20250624235635.png]]

Registration
![[Pasted image 20250624235753.png]]

3D Data Classification -- 3D scene understanding (task of semantization - also referred as classification)
1. 3D object detection (bounding-box techniques -- enable the system to capture objects' sizes, orientations, and positions in the world)
2. 3D semantic segmentation (assigning semantic labels to every base unit)
3. 3D instance segmentation (semantic segmentation step on mega-steroids)
![[Pasted image 20250625000336.png]]

Structuration/Modelling (data is organized in a way that allows for easy manipulation and understanding)
3D Data Analysis (to describe the data accurately, understand trends, and make inferences)
3D Data Visualization (makes it easier for people to grasp complex information by enhancing the capacity to present the data effectively)


![[Pasted image 20250625001312.png]]
