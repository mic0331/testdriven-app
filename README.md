# Microservices with Docker, Flask, and React

[![Build Status](https://travis-ci.org/mic0331/testdriven-app.svg?branch=master)](https://travis-ci.org/mic0331/testdriven-app)


This is a proof of concept project where the objective is to build a code evaluation tool for grading code exercices, similar to Codeacademy, with Python, Flask and JavaScript, ReactJS.
The app itself, will allow a user to log in and submit solutions to a coding problem. They will also be able to get feedback on whether a particular solution is correct or not.

The main purpose of this project is to dive into Docker and container orchestration to help manage, scale, and deploy a fleet of microservices.

Some useful commands:

1. start a service
```
    $ docker-compose -f docker-compose-dev.yml up -d
```

2. get the machine IP
```
    $ docker-machine ip testdriven-dev
```

3. create the container

```
    $ docker-machine create -d virtualbox testdriven-dev
```

1. Test a specific module

```
    $ docker-compose -f docker-compose-dev.yml run users-service python manage.py test
```


