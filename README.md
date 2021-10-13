# ros2-vnc

Extends [this](https://github.com/bandi13/gui-docker)

I build with 
> docker build . -t foxy:vnc


I run the docker with:
> docker run --shm-size=256m -it -p 5901:5901 -e VNC_PASSWD=123456   foxy:vnc

To access the vnc server go to the noVNC client url in your favorite browser. On macOS, you may need to replace the provided ip address (not the port) with "localhost".
