# OS
This is the reporitoty of my PintOS project

# Solution
The actual solution is located inside threads/thread.c file in the thread_yield function

# Installation

To verify that the base-image is installed (if not, install) and run it:
```
docker run -it pkuflyingpig/pintos bash
```

To launch a Docker container and mounted volume:
```
git clone https://github.com/seelennebel/OS.git
docker run -it --rm --name pintos --mount type=bind,source=absolute/path/to/OS with src directory/on/your/host/machine,target=/home/PKUOS/pintos pkuflyingpig/pintos bash
```

Inside PintOS:
```
cd  src/threads
make
cd build
pintos --bochs -- run alarm-priority
```
