# manipulator_rviz  
Repo with new URDF of manipulator to visualize in RViz and using command line as well as gui to give input to RViz  
### Steps to run the demo  

* Create a new catkin workspace

```
  source /opt/ros/noetic/setup.bash
  mkdir -p ~/catkin_ws/src
  cd ~/catkin_ws/
  catkin_make
  source devel/setup.bash
```

*  Clone this repo
```
  cd ~/catkin_ws/src
  git clone https://github.com/MOLOCH-dev/manipulator_rviz.git 
```
  
  
*  Rebuild
```
  cd ~/catkin_ws
  catkin_make
```
*  Run the launch file
```
  oslaunch manipulator_description display.launch 
```
   *  If you come across this error  
Could not find the GUI, install the 'joint_state_publisher_gui' package  
   *  Install  using  
sudo apt install ros-<your_version_of_ros>-joint-state-publisher-gui 
----------------------------------------------------------------------  
  
*  Once you are done with the visualisation with gui , Ctrl+ c to stop this .  
  
  
*  For command line input    
    *  roslaunch manipulator_rviz new.launch    
    *  Now ,On a different terminal  
    cd/manipulator_rviz  
    *  python pub_try1.py  
Then initially set all values to zero , to get the default position of the manipulator .  
After this you can now check for different values.
