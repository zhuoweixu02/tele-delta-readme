# tele-delta-readme
this is  a readme for how to use the delta

## plug source cable
1. open the top switch(the lower one is for another robot)
2. plug the source cable for delta and the pie

## start the robot
1.  run `roscore` to start the ros
2.  run `ssh -X iam-lab@iam-reality` to connect the slave pc
3.  run `google-chrome` or open the chrome, Address `172.16.0.2` to open the control padel, if everything works on well the color bar shall be yellow.
4.  click on "Click to unlock", the color bar will turn to pink
5.  press the E-stop button, the color bar turn to white
6.  twist the E-stop button, the color bar tuen to blue. If press again, it will turn white.

## start tele-hand and delta-hand
1. run `./bash_scripts/start_control_pc.sh -i iam-reality` under the path of `Documents/frankapy`
2. run `python initialize_franka.py -c tabletop -block` under the path of `Documents/Delta-robot/teleoperation-slider`, run sfranka under same path to activate environment franka
4. run `ssh zilinssi@nema` to start the cam
5. run `roslaunch rosserial-hand.launch` under the path of `Documents/Delta-robot/teleoperation-slider`
6. enabling teleoperation, run `python slider-control.py -d -c` under the same path, but another terminal
