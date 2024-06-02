# hello-world

A Hello World webpage created completely using Github Co-Pilot.

This project contains a simple "Hello World" webpage that is served using a Docker container. The webpage is created using HTML and the Docker container uses an Nginx image to serve the webpage.

To view the webpage, follow these steps:

1. Ensure Docker is installed and running on your machine. If not, you can download Docker from [here](https://www.docker.com/products/docker-desktop) and follow the instructions to install and run it.

2. Clone this repository to your local machine.

3. Navigate to the project directory in your terminal.

4. Build the Docker image using the following command:
    ```bash
    docker build -t hello-world-webpage .
    ```

5. Run the Docker container using the following command:
    ```bash
    docker run -p 8080:80 hello-world-webpage
    ```

6. Open your web browser and navigate to `http://localhost:8080`. You should see the "Hello World" webpage.

Please note that the Docker container is configured to use port 8080. If this port is already in use on your machine, you can change the port mapping in the `docker run` command. For example, to use port 9090 instead, the command would be `docker run -p 9090:80 hello-world-webpage`, and you would navigate to `http://localhost:9090` in your web browser.
