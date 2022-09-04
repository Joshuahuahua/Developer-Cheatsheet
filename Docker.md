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
`-t` applies a tag, so image can be referenced.  
`.` refers to the Dockerfile path (run at project root)  
``docker build -t IMAGE-NAME .``  

**Run Container**  
`docker run IMAGE-NAME`  
Use "-e" to pass through environment variables ("TERM" has been used as an example)  
`docker run -e TERM=xterm IMAGE-NAME`  

## Useful Commands  
**Run python virtual env**  
`venv/Scripts/Activate.ps1`  

**Write current pip env packages to file**  
`pip freeze > requirements.txt`  