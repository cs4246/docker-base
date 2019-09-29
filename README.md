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
```
### Linux / Mac
```
docker run -it --rm -v $PWD:/workspace cs4246/base <command>
```
### Windows
```
docker run -it --rm -v %cd%:/workspace cs4246/base <command>
```

## Examples

For example, if you want to run ``python train.py`` inside ``/home/cs4246/hw1``, you can do:

```
cd /home/cs4246/hw1
```

### Linux / Mac
```
docker run -it --rm -v $PWD:/workspace cs4246/base python train.py
```
### Windows
```
cd /home/cs4246/hw1
docker run -it --rm -v %cd%:/workspace cs4246/base python train.py  
```
