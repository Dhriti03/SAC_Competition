
1. Extract contents of "sac_final_2022" folder to `<workspace>/src/`

2. Copy the following folders to .gazebo/models
   mkdir .gazebo/models/arena
   mkdir .gazebo/models/markerfinal
   cp <workspace>/src/sac_final_2022/meshes/final_arena.dae .gazebo/models/arena/arena_final.dae
   cp final_ws/src/sac_final_2022/meshes/Marker0.png .gazebo/models/markerfinal/Marker0.png
   cp <workspace>/src/sac_final_2022/meshes/Markerfinal.dae .gazebo/models/markerfinal/Markerfinal.dae

3. Open terminal from your <workspace> and do
      ```
   catkin_make
   source devel/setup.bash
   roslaunch sac_final_2022 launch_arena.launch
   ```

**NOTE**: If there is a error saying `Error [Converter.cc:127] Unable to convert from SDF version 1.6 to x.x`. Just change the sdf version in line `1` of `final_arena.world`
