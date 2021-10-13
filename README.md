# ros2-vnc

Extends [this](https://github.com/bandi13/gui-docker)

I build with 
> docker build . -t foxy:vnc


I run the docker with:
> docker run --shm-size=256m -it -p 5901:5901 -e VNC_PASSWD=123456 --name foxy-vnc  foxy:vnc

Then access it with:
> http://localhost:5901/?password=123456

Once you start this, you'll see a _mostly blank looking_ vnc window.  You can either right click to access the menu and open a terminal, OR, if you don't have an right click (Apple hardware I'm looking at you):

You can then start *another* docker container:

> docker exec -it foxy-nvc bash
source ROS:w

> source /opt/ros/fox/setup.bash

set the display environment variable:

> export DISPLAY=:0

