
# Introduction to Flutter
* **An SDK** that makes building high-performance, modern, and beatiful apps easy
* Work natively for both Andorid and iOS - not a wrapper
* Uses the **Dart** programming language

### Notice 
It is made by Google.
Reference https://flutter.dev/?gclid=Cj0KCQiA9P__BRC0ARIsAEZ6irj1tGvjNM5CfJ4TMgtSyhqGzBtnKBB9PAW9EMUgRWYGOU0nsM203WAaAme2EALw_wcB&gclsrc=aw.ds

### Advantages
* Create your UI **quickly** - low learning curve
* Use plug-ins & packages for easy interactions with platforms hardware
* Build once and deploy to multiple platforms
* **Hot Reload** when designing

### Not A Fit for Rapid Prototyping
games, calling native APIs directly, audio support, new.different third-party libraries, watches, TVs, Cars

### Examples
```dart
void main() {
    runApp(
        Center(
    
```


# Introduction to Docker
* Docker is a tool that makes it really easy to package applications into self-sustaining 'cotainers'

### Container
Containers contain libraries, dependencies and source codes.

### Advtanges
* Easily get the benefits of containers
* Programmatically define containers

### Docker Containers
A Docker containers is a fully self-contained and running version of your application


### Docker Images
Images are tmeplates that describe to Docker how to create a container from scratch.

### Docker Layers
Layers are resuable components that can be shared accross images

### Dockerfile
The dockerfile is the actual instruction manual that sell Docker how to build your image. This is the only part you as a user write

### Docker CLI
```bash
$ docker run hello-world
```

### docker build 
```bash
# turn a Dockerfile into an actual image
$ docker build . -t node-example:latest
```

### Docker image ls
```bash
# get a list of all images you have in your computer
$ docker image ls
```

### docker run
```bash
# create a container from an image
$ docker run -p 3000:3000 node-exampe:latest

# Then run node in the curent directory
$ node .
```

### Note
Bedore you head to the next run, you should fisrt kill the running project
* steps
```bash
# find the container ID
$ docker ps
CONTAINER ID   IMAGE                 COMMAND                  CREATED         STATUS         PORTS     NAMES
4038a055a929   node-example:latest   "docker-entrypoint.s…"   2 minutes ago   Up 2 minutes             magical_zhukovsky

# then kill the container
$ docker kill 4038a055a929
```


### docker exec
```bash
# how to run a command inside a container
$ docker exec -it 4038a055a929 echo "Hello Hack the north 2020++"

# list of current runnning
$ dcker exrc -it 4038a055a929 ps aux 

# intereact with shell
$ docker exec -it 4038a055a929 /bin/sh
```


### Deploying on GCR (Google Cloud Run)
Docker makese it dead easy to deploy on pretty much any cloud platform on the internet. 

# References
https://www.youtube.com/watch?v=rgfezE92mog&feature=youtu.be
