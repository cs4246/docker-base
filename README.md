# CS4246 Docker Base

Docker image with built-in environment and simulator for CS4246 course.

## Usage

Pull the image:
```
docker pull cs4246/base
```

Run your program inside the container:
```
cd /path/to/your/program
docker run -it --rm -v $PWD:/workspace cs4246/base <command>
```

For example, if you want to run ``python train.py`` inside ``/home/cs4246/hw1``, you can do:
```
cd /home/cs4246/hw1
docker run -it --rm -v $PWD:/workspace cs4246/base python train.py
```
