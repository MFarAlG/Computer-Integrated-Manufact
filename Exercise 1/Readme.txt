The code was written using Python script in Blender. Below is the description of the code.

import bpy - Imports the Blender Python module.
bpy.ops.mesh.primitive_cube_add(size=1) - Adds a cube to the Blender scene. The size parameter sets the size of the cube.
box1 = bpy.context.active_object - Assigns the newly created cube to the variable box1.
box1.scale = (1, 1, 1) - Sets the scale of box1 to (1, 1, 1).
box1_location = (3, 0, 0) - Sets the location of box1 to (3, 0, 0).
box1.location = box1_location - Assigns the location of box1 to box1_location.
bpy.ops.mesh.primitive_cube_add(size=1) - Creates a new cube for the lid.
lid1 = bpy.context.active_object - Assigns the newly created lid to the variable lid1.
lid1.scale = (1.1, 1.1, 0.2) - Sets the scale of lid1 to (1.1, 1.1, 0.2).
lid1_location = (3, 0, 0.5) - Sets the location of lid1 to (3, 0, 0.5).
lid1.location = lid1_location - Assigns the location of lid1 to lid1_location.

The above code is to create only a single box. To create multiple box, we duplicated the code 2 times and adjust the location and scale of the box. Hence we could get 3 boxes with different size and location.

