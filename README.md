# PlatformEngineerJourney

## Introduction

Hello! My name is [Your Name], and I am a software testing professional with basic knowledge of Python and SQL. This repository will document my journey as I transition into a platform engineering role. I will be updating this space with my progress, projects, and any valuable resources I come across.

## Current Skills

- Software Testing
- Basic Python
- Basic SQL

## Goal

To become a proficient Platform Engineer by building on my existing skills, gaining new knowledge, and completing hands-on projects.

## Progress

### Step 1: Setting Up GitHub

- Created a GitHub account.
- Set up a new repository named `PlatformEngineerJourney`.
- Initialized the repository with a README file.
- Added a brief introduction and outlined current skills and goals.

### Step 2: Introduction to Docker

- Learned the basics of Docker by reading [Docker Overview](https://docs.docker.com/get-started/overview/) and [Docker for Beginners](https://www.docker.com/101-tutorial).
- Installed Docker on my local machine.
- Pulled and ran the "hello-world" Docker image to verify the installation.

#### Commands Run

- Pulled the "hello-world" Docker image:
  ```sh
  docker pull hello-world

### Step 3: Build a simple python application using docker

- Create a folder
- create a file app.py, enter a print statement and save the file.
- create a file called docker file with the below code to containerize the application
  
  ```
    # Use the official Python base image
      FROM python:3.9-slim

    # Set the working directory in the container
      WORKDIR /app

    # Copy the current directory contents into the container at /app
      COPY . /app

    # Run app.py when the container launches
      CMD ["python", "app.py"]

  ```
- Go to Command prompt and execute the command to build docker image for the python app.
  ```
    docker build -t python-hello-docker .
  ```
- Execute docker run to run the container
  ```
    docker run python-hello-docker
  ```
  

