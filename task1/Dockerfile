# Use the latest Ubuntu as the base image
FROM ubuntu:latest

# Update APT and install Python3, Python3-pip and Flask
RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y python3 python3-pip
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED
RUN pip3 install flask

#Create Location (-p don't create if already exists)
RUN mkdir -p /app

# Copy the python file to your Docker image
COPY ./api.py /app/api.py

# Use /app as your working directory
WORKDIR /app

# Run the python file
CMD python3 api.py
