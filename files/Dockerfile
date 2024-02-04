# Dockerfile

# Author       : Adrayle
# Github       : https://github.com/adrayleebon
# Email        : adrayle19@gmail.com
# Main Language: Python

# Download and import main images

# Operating system
FROM debian:latest
# Main package
FROM python:3

# Author info
LABEL MAINTAINER="https://github.com/adrayleebon/AdrayleP"

# Working directory
WORKDIR /PyPhisher/
# Add files 
ADD . /PyPhisher

# Installing other packages
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install python3-pip php openssh-client -y
RUN pip3 install -r files/requirements.txt --break-system-packages
RUN apt-get clean

# Main command
CMD ["python3", "AdrayleP.py", "--noupdate"]
