#set base image for docker
FROM python:3.9.1

#install libraries
RUN apt-get install wget
RUN pip install pandas sqlalchemy psycopg2

#set working directory
WORKDIR /app
#copy pipeline.py from host machine to app
COPY pipeline.py pipeline.py

#set entry point for docker container(command that run when docker start)
ENTRYPOINT ["python", "pipeline.py"]

 