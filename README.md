# mini_cheetah_pybullet
mpc and wbc for mini cheetah in pybullet
mpc forked from https://github.com/Derek-TH-Wang/quadruped_ctrl
we added the wbc to climb the stairs, since the mpc cannot climb the stairs.

System requirements:
Ubuntu 16.04

Running:

run the controller in simulator:

rosrun quadruped_ctrl walking_simulation.py

roslaunch quadruped_ctrl quadruped_ctrl.launch

stand:
rosservice call /robot_mode "cmd: 1"

trot:
rosservice call /robot_mode "cmd: 4"

you can switch the gait type:

rosservice call /gait_type "cmd: 1"
gait type:

0:trot
1:bunding
2:pronking
3:random
4:standing
5:trotRunning
6:random2
7:galloping
8:pacing
9:trot (same as 0)
10:walking
11:walking2
