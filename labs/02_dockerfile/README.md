Build Instructions
==================
Change into the newly created directory. Then run:

    podman build -t oracle/dockerfiledemo:latest .

After doing so, you will have built the image. To run the example run:

    podman run --rm oracle/dockerfiledemo:latest

Another example of docker run which will start new containers each time it is run based on image specified

    podman run --rm -it oracle/dockerfiledemo:latest sh
    # touch file1

    podman run --rm -it oracle/dockerfiledemo:latest sh
    # touch file2


docker exec lets you run commands on an already running container!

    docker exec -it <container-id> <command to execute in container>
    docker exec -it 9675901 sh

    docker run --rm -it oracle/dockerfiledemo:latest sh
