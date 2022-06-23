# Turtle Pong

This repository hosts the source code for the ROS `turtle_pong` package which 
implements the Pong arcade video game for the Robot Operating System (ROS 1 Noetic) using turtlesim.

![Short Game Play](docs/turtle_pong.gif)

## Set up

Install turtlesim package
```
sudo apt-get install ros-noetic-turtlesim
```

turtlesim package contains 3 nodes try running all of them and explore what they do.

# Assignment

Create a new catkin workspace. Clone this package inside the src of your workspace.

src of the package contains 3 nodes that needs to be execute at a time. So create a launch file `node.launch` to execute these 3 files(Executable is the filename without extension) at a time.

After the launch file is created, you have to run the node `turtlesim_node` and the launch file `node.launch`

Inspect the create nodes and their topics using the following commands:

* `rosnode list`
* `rostopic list`
* `rosservice list`
* `rosnode info [NODE]`
* `rostopic echo [TOPIC]`
* `rossrv show [TYPE]` 
* `rosmsg show` 
* `rostopic info [TOPIC]`
* `rosservice info [SERVICE]`

Execute `rqt_graph`. Take a screenshot of the resulting graph.
* Display only active nodes/topics.
* Remember to press the button next to ‘Fit’ for a properly viewable
graph.

Use `rosbag` record to record data from the odometry topic (Find the
exact topic name using the graph.) Once you have started recording,
execute the publish command. Stop the recording after 10 seconds.

## Submission

Make a new folder named `submission` inside the package place your bag recording and the screenshot inside it and create a PR. 