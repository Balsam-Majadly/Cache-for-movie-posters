
# A cache for movie poster- Dockerized Flask Mongo App Project

This project demonstrates how to containerize a Flask web application with a MongoDB database using Docker. It provides a basic setup for running a Flask app with MongoDB in a Docker environment.This app project enables programmatic access via the internet to a database of images (movie posters). The database is based on MongoDB and stores movie files and information about the files (movie title, IMDB code, etc.). The software is based on Flask. Both the software and the database should be "wrapped in containers",we used docker-compose.

## Features

- Dockerized Flask web application
- Integration with MongoDB database
- Docker Compose for easy container orchestration
- Basic user authentication and CRUD operations
- API endpoints for interacting with the database

## Prerequisites

Make sure you have the following prerequisites installed on your machine:

- Docker: [Install Docker](https://docs.docker.com/get-docker/)
- Docker Compose: [Install Docker Compose](https://docs.docker.com/compose/install/)

## Getting Started

To get started with this project, follow these steps to run this app in your local environment:

1. Clone the repository:


git clone https://github.com/Balsam-Majadly/Cache-for-movie-posters.git


2. Change to the project directory:


cd Cache-for-movie-posters/

3. make api key https://www.themoviedb.org/login
   
5. create a file, and add your api key
   
  echo "api_key = 'your api key'" > config.py
  
7. Build and start the Docker containers:


docker-compose up -d


4. Open your web browser and access the application at `http://localhost:5000`.

or you can run this app in your ec2 instance:

1.create ec2 

2.make sure to add inbound rules to allow incoming traffic on ports 5000 and 8081 in a security group associated with your EC2 instance

3.make sure to add user data, you can copy from this link
https://github.com/Balsam-Majadly/Cache-for-movie-posters/blob/main/user_data.txt




## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvement, please feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).



Please note that the generated README file is a starting point and you may need to customize it further based on your specific requirements and project details.
