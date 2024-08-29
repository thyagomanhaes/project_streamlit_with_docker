## How to run this project on your local machine

Packages used in this project:

- python 3.11.5
- pyenv: to manage the python versions
- poetry: to create the project

Follow this steps to run on your local machine:

First of all, you have to install Docker Desktop, if you're using a Windows machine.

Assure that docker is running, go to your workspace directory and run the following commands on your terminal (I use Git Bash):

```
docker build -t my-project-image .
```

After the Docker image was created, you can run a container using this image:

```
docker run -d -p 8501:8501 --name my-container-name my-project-image
```

If everthing goes well, you can access the app in your browser in 
"localhost:8051"

_This simple project is just a glance to see a docker container running a Python application. You can push this image to Dockerhub for example and use Kubernetes to manage a lot of containers for your project._

