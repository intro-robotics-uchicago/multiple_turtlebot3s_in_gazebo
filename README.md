# multiple-turtlebot3s-in-gazebo

This ROS package gives an example launchfile that launches 3 Turtlebot3 robots in the same world. 

## Running the code

To run the code execute `roscore` in one terminal and then run the following command in a separate terminal: 

```
roslaunch multiple_turtlebot3s_in_gazebo multiple_turtlebot3s_in_empty_world.launch
```

Once you run the launchfile which spawns 3 Turtlebot3 robots, you can run `rostopic list` in a third terminal to see the list of ROS topics: 

```
/clock
/gazebo/link_states
/gazebo/model_states
/gazebo/parameter_descriptions
/gazebo/parameter_updates
/gazebo/set_link_state
/gazebo/set_model_state
/rosout
/rosout_agg
/tb3_0/camera/parameter_descriptions
/tb3_0/camera/parameter_updates
/tb3_0/camera/rgb/camera_info
/tb3_0/camera/rgb/image_raw
/tb3_0/camera/rgb/image_raw/compressed
/tb3_0/camera/rgb/image_raw/compressed/parameter_descriptions
/tb3_0/camera/rgb/image_raw/compressed/parameter_updates
/tb3_0/camera/rgb/image_raw/compressedDepth
/tb3_0/camera/rgb/image_raw/compressedDepth/parameter_descriptions
/tb3_0/camera/rgb/image_raw/compressedDepth/parameter_updates
/tb3_0/camera/rgb/image_raw/theora
/tb3_0/camera/rgb/image_raw/theora/parameter_descriptions
/tb3_0/camera/rgb/image_raw/theora/parameter_updates
/tb3_0/cmd_vel
/tb3_0/imu
/tb3_0/joint_states
/tb3_0/odom
/tb3_0/scan
/tb3_1/camera/parameter_descriptions
/tb3_1/camera/parameter_updates
/tb3_1/camera/rgb/camera_info
/tb3_1/camera/rgb/image_raw
/tb3_1/camera/rgb/image_raw/compressed
/tb3_1/camera/rgb/image_raw/compressed/parameter_descriptions
/tb3_1/camera/rgb/image_raw/compressed/parameter_updates
/tb3_1/camera/rgb/image_raw/compressedDepth
/tb3_1/camera/rgb/image_raw/compressedDepth/parameter_descriptions
/tb3_1/camera/rgb/image_raw/compressedDepth/parameter_updates
/tb3_1/camera/rgb/image_raw/theora
/tb3_1/camera/rgb/image_raw/theora/parameter_descriptions
/tb3_1/camera/rgb/image_raw/theora/parameter_updates
/tb3_1/cmd_vel
/tb3_1/imu
/tb3_1/joint_states
/tb3_1/odom
/tb3_1/scan
/tb3_2/camera/parameter_descriptions
/tb3_2/camera/parameter_updates
/tb3_2/camera/rgb/camera_info
/tb3_2/camera/rgb/image_raw
/tb3_2/camera/rgb/image_raw/compressed
/tb3_2/camera/rgb/image_raw/compressed/parameter_descriptions
/tb3_2/camera/rgb/image_raw/compressed/parameter_updates
/tb3_2/camera/rgb/image_raw/compressedDepth
/tb3_2/camera/rgb/image_raw/compressedDepth/parameter_descriptions
/tb3_2/camera/rgb/image_raw/compressedDepth/parameter_updates
/tb3_2/camera/rgb/image_raw/theora
/tb3_2/camera/rgb/image_raw/theora/parameter_descriptions
/tb3_2/camera/rgb/image_raw/theora/parameter_updates
/tb3_2/cmd_vel
/tb3_2/imu
/tb3_2/joint_states
/tb3_2/odom
/tb3_2/scan
/tf
/tf_static
```

As you can see, there is one set of topics for each of the three Turltlebot3 robots, where each Turtlebot3 robot has it's own unique prefix (`tb3_0`, `tb3_1`, `tb3_2`). 

## Acknowledgements

This code was adapted from [takahub1's multi_turtlebot3.launch](https://gist.github.com/takahub1/85cb995b3c9d7a7008f31dc900092b04).