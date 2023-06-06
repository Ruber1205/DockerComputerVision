# Docker Computer Vision Project
Universidad Nacional de Colombia Sede Medellín - Facultad de Minas

## How to run and play with the project? ##

This project is wrapped on a Docker container to run a jupyter-lab environment. Make sure that you have docker installed in your machine. Open the OS Terminal and then execute the [`build`](./docker_scripts/build) script once to create the container and [`run`](./docker_scripts/run) always:

```
$ # build to create the container (just need to be executed only once)
$ ./docker_scripts/build
$ # run to execute the jupyter-lab container
$ ./docker_scripts/run
```

Once the docker container is running, open your web browser and go to http://localhost:8899. The password required is `unal2021`.

## Windows ##

Build the container
```
$ docker build -t computer_vision ./

```

Run the container
```
docker run -it -p 8899:8899 --name=computer_vision --volume ${PWD}/ComputerVisionProject:/ComputerVisionProject --hostname=cvproject.local --rm computer_vision
```

