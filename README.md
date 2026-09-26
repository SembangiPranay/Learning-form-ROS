# Learning-form-ROS
I will be updating my learning of ROS 2 (Lyrical)

1. Why 'colcon build' & 'source install/setup.bash' ?
ans:- In a ROS 2 workspace, colcon build is used to compile/build the packages present inside the src folder and generate the required files in the build, install, and log folders. 
After building, source install/setup.bash is used to load the newly built workspace into the current terminal environment so that ROS 2 can find and run the packages and nodes created in that workspace. 
Thus, the usual workflow is write/create package → colcon build → source install/setup.bash → run the node.

2. what are packages and excutables ?
ans:- In ROS 2, think of a package as a container/folder that groups everything needed for a particular piece of functionality—such as source code, configuration files, dependencies, and executables. An executable is an actual program inside that package that you can run. For example, the turtlesim package contains executables such as turtlesim_node; when you type ros2 run turtlesim turtlesim_node, turtlesim is the package and turtlesim_node is the executable. So the basic relationship is: Package → contains executables → executables run as ROS 2 nodes.
