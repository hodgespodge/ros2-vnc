# ros2-vnc

I build with 
> docker build . -t foxy:vnc


I run the docker with:
> docker run --shm-size=256m -it -p 5901:5901 -e VNC_PASSWD=123456   foxy:vnc
