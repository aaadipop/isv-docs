## Docker cheat sheet

1. Builds an image from a Dockerfile in the current directory

    ```bash
    docker build
    ```

2. Builds an image with the specified name "image_name" using the Dockerfile located in the current directory indicated by "."
   
    ```bash
    docker build -t image_name .
    ```

3. Starts a new container

    ```bash
    docker start container
    ```

4. Stops a container

    ```bash
    docker stop container
    ```

5. Lists all running containers

    ```bash
    docker ps
    ```
   
6. Lists all containers

    ```bash
    docker ps -a
    ```

7. Execute an interactive shell on the container

    ```bash
    docker exec -it container /bin/sh
    ```

8. Runs the container named "my_container" in detached mode, maps port 8080 on the host to port 80 in the container, based on the specified image.

    ```bash
    docker run -d -p 8080:80 --name my_container image_name
    ```


## Linux cheat sheet

1. Display information about the operating system distribution

    ```bash
    cat /etc/os-release
    ```
   
2. Edit filename starting at line 1

    ```bash
    vi filename	 
    ```
   
3. **i** - insert text before cursor, until <Esc> hit
4. **:wq<Return>** - quit vi, writing out modified file to file named in original invocation

