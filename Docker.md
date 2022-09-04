# Docker

## "Dockerfile"  
**Select OS/Environment (python:3.9)**  
`FROM WORKING-ENVIRONMENT`  
**Name virual working directory**  
`WORKDIR /VIRTUAL-APP-DIR`  
**ADD/COPY files/folders**  
`COPY FILENAME .`  
`COPY FILENAME ./VIRTUAL-FOLDER`  
**Install Dependancies (PYTHON Example)**  
`RUN pip install PACKAGE-NAME`  
`RUN pip install -r requirements.txt`  
**Run Application (Python)**
`CMD ["python", "./FILENAME.py"]`  

## Deployment  
**Build Container Image**  
`-t` applies a tag, so image can be referenced  
`.` refers to the Dockerfile path (run at project root)  
``docker build -t IMAGE-NAME .``  
**Run Container**  
`docker run IMAGE-NAME`  
`-e` is used to pass through environment variables ("TERM" has been used as an example)  
`docker run -e TERM=xterm IMAGE-NAME`  
`-v` mounts a volume to a directory on the host machine  
`docker run -v VOLUME-NAME:/PATH-TO-DIR getting-started`  

## Useful Commands  
**List Containers**  
`docker ps`  
**Stop Container**  
`docker stop CONTAINER-ID`  
**Remove Container**
`docker rm CONTAINER-ID`  
`-f` can be used to force remove a container (even while it is running)  
`docker rm -f CONTAINER-ID`  

**Create Named Volume**  
`docker volume create FILENAME`  

**Run python virtual env**  
`venv/Scripts/Activate.ps1`  
**Write current pip env packages to file**  
`pip freeze > requirements.txt`  