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

## Task 1
Create a new catkin workspace. Clone this package inside the src of your workspace.

## Task 2
src of the package contains 3 nodes that needs to be executed. Register all 3 nodes as an executable by editing the `CMakelists.txt`.

## Task 3
The package depends on 
* std_msgs
* std_srvs

Check whether they are added as dependencies, if not add them.

## Task 4
We need to execute the 3 nodes together, so create a launch file `node.launch` to execute these 3 files at a time.

After the launch file is created, you have to run the node `turtlesim_node` and the launch file `node.launch`

## Task 5
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


## Task 6
Execute `rqt_graph`. Take a screenshot of the resulting graph.
* Display only active nodes/topics.
* Remember to press the button next to ‘Fit’ for a properly viewable
graph.

## Task 7
Use `rosbag` record to record data from the odometry topic (Find the
exact topic name using the graph.) Once you have started recording,
execute the publish command. Stop the recording after 10 seconds.

## Submission

Make a new folder named `submission` inside the package place your bag recording and the screenshot inside it and create a PR. 