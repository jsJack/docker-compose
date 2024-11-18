# Docker-Compose Repository

Welcome to my Docker-Compose repository! This repository contains a collection of Docker Compose files that I use to manage my personal infrastructure. You can use these files to set up and manage your own Docker containers with ease.\

Feel free to use them as starting points for Docker projects, or to quickly setup an app, like one I've used before. Don't feel like you need to credit me in any way to use them, but if you make a public article about them, I'd appreciate you linking them back to the [original repo](https://github.com/jsJack/docker-compose).

## Repository Structure

The repository is organized as follows:

```
docker-compose
    ├── service1
    │   └── docker-compose.yml
    │   └── .env.example
    ├── service2
    │   └── docker-compose.yml
    └── ...
```

Each directory contains a `docker-compose.yml` file for a specific service.\
Some services may also contain a `.env.example` file, you can clone this using `cp .env.example .env` and filling out the details as necessary.

## Usage

To use these Docker Compose files on your own infrastructure, follow these steps:

1. Clone the repository to your desired location:
    ```bash
    git clone https://github.com/jsJack/docker-compose.git /opt/docker-compose
    ```

2. Navigate to the directory of the service you want to run:
    ```bash
    cd /opt/docker-compose/service1
    ```

3. Fill out the environment variable file:
    ```bash
    cp .env.example .env
    nano .env
    ```

4. Start the service using Docker Compose:
    ```bash
    docker-compose up -d
    ```

5. Voilà! 🐳

## Contributing

If you have any improvements or additional services you'd like to add, feel free to open a pull request or create an issue.

## License

This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

Happy Dockerizing!