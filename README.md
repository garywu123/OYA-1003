# OYA-1003
Automated Guided Vehicle simulation

Place the files under the catkin_ws / src file. The "workcell" and "workcell_bin" files are model files.
To be able to add these models to the world easily add this command to bashrc file.
#### $ export GAZEBO_MODEL_PATH=/home/[kullanıcı adınız]/catkin_ws/src 
To run the world, 
#### $ cd ~/catkin_ws
#### $ catkin_make
#### $ source catkin_ws/devel/setup.bash
#### $ roslaunch agvcasterwheel_gazebo agvcasterwheel.launch 
write this commands to terminal.

Ariac environment is using in this simulation there are three AGV 's on this simulation called agv1, agv2 and agv3.
Each topic starts with robots name.(/agv1/sonar1)

If you want to change the starting positions of the robot, change "x","y" parameters on the agvcasterwheel.launch file and 
if you want to change the head angle, change "yaw" parameter on the agvcasterwheel.launch file.

##### You should publish cmd_vel topics of robots in different terminals.\

Robot components:
                  1 base frame,\
                  4 caster base,\
                  4 caster,\
                  2 tire,\
                  2 wheel,\
                  4 Bumper sensors,\
                  1 kinect sensor,\
                  10 Sonar sensors: ranges are 0-5 meter.\
                                    update rates is 100.(approximately 2 in a second).\               
                  2 Hokuyo Laser sensors: ranges are 0-30 meter.\
                                          update rate is 40. (approximately 1 in a second).\
                                          
Environment is taken from Ariac competition environment.               \
Environment features: \
                     width x height = 20.25 x 20.25,\
                     3 automated guided vehicle.\
                     1 m width robot path,\
                     1.5 m width robot path,\
                     2 m width robot path.\
                      
