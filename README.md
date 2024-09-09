# Bookmark Website

This project sets up a simple bookmark website using two Nginx containers. The site contents are served from local directories on your machine.

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Project Structure

The project structure is as follows:


- `site/`: Contains the HTML files for the first website.
- `site1/`: Contains the HTML files for the second website.
- `docker-compose.yml`: Docker Compose file that defines the services.

## Usage

1. **Clone the Repository**

   Clone this repository to your local machine or set up your file structure as described above.

2. **Navigate to the Project Directory**

   ```bash
   cd /root/bookmark-website/

docker-compose up -d


Accessing the Website
First Website: Open your web browser and go to http://localhost:9000 to access the first bookmark website.

Second Website: Open your web browser and go to http://localhost:9005 to access the second bookmark website.

Stopping the Containers
To stop the running containers, navigate to the project directory and run:

docker-compose down

Troubleshooting
Container Logs: If you encounter any issues, you can view the logs for a container using:

docker-compose logs web
docker-compose logs web2

Rebuilding Containers: If you make changes to the docker-compose.yml or Dockerfile, rebuild the containers with:
docker-compose up -d --build

License
This project is open-source and available under the MIT License.

This README provides a comprehensive guide to setting up, running, and customizing the bookmark website using the provided Docker Compose configuration.
