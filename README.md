# docker-flatten

`docker-flatten` is a tool that allows you to flatten Docker images by removing unnecessary layers, turning your container's filesystem into a single pristine layer. This helps reduce image size and removes bloat that accumulates over time.

## Features

- Export a running container's filesystem and create a new image from it
- Strip away Docker image layers to create a clean, minimal base
- Simple and efficient for creating optimized Docker images without needing a Dockerfile

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/<your-username>/docker-flatten.git
    ```

2. Navigate to the repository:
    ```bash
    cd docker-flatten
    ```

3. Make the script executable:
    ```bash
    chmod +x docker-flatten
    ```

4. Optionally, move it to a directory in your PATH for easy access:
    ```bash
    sudo mv docker-flatten /usr/local/bin/
    ```

## Usage

To flatten an image and create a new minimal image, run the following command:

```bash
docker-flatten <source-image> <new-image-name>
