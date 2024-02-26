Build Instructions
==================
Change into the newly created directory. Then run:

    docker build -t tah/helloworld:latest .

docker run is the command you use to create a new container from an image

    docker run --rm -t tah/helloworld:latest

docker exec lets you run commands on an already running container!

    docker exec -it <container-id> <command to execute in container>
    docker exec -it 9675901 sh

    ls