# 🤗 huggingface fastapi docker github container

create a container and package it with GitHub Actions. This repository gives you a good starting point for a Dockerfile, GitHub Actions workflow, and Python code.

The web application uses FastAPI with Hugging Face and exposes a single endpoint that you can interact with it. 

open codespaces on github project menu
open new terminal window
check if docker installed
> docker ps
> check the project directory
>ls
build docker file from Dockerfile in the project folder
>docker build -t local-ml-model-serve .
check image 
> docker image ls
run the docker 
>docker run -p 8000:8000  --name hugging-fastapi local-ml-model-serve

confirm popup window to open a new page
refresh a couple of times

and you will see "A self-documenting API to interact with a GPT2 model and generate text"
now go to endpoint /docs to see fast api info
go to post section and try out

change text body and execute to see response. That's it.



Now we can work with github actions
first select repo settings and scroll down below to "Workflow permissions" and select "read write permissons" and click "save"
Select actions from github menu above.
select Docker image for configuration,and edit it as main.yml accordingly

then go to actions tab and select newly created workflow "CI" from left paneland `run workflow`




