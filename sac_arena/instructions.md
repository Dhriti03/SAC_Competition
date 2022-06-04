
1. Copy `arena_with_qr` folder to `<workspace>/src/`

2. Copy the following folders to .gazebo/models
   mkdir .gazebo/models/arena
   cp <workspace>/src/models/arena_samplenew.dae .gazebo/models/arena/
   cp <workspace>/src/models/marker10 .gazebo/models/

3. Open terminal from your <workspace> and do
      ```
   catkin_make
   source devel/setup.bash
   roslaunch arena_with_qr launch_in_gz.launch
   ```

**NOTE**: If there is a error saying `Error [Converter.cc:127] Unable to convert from SDF version 1.6 to x.x`. Just change the sdf version in line `1` of `cubes_and_qr.world`