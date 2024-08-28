# latest version of Ubuntu 
FROM ubuntu:latest

# Update  list 
RUN apt-get update

# Upgrade 
RUN apt-get upgrade -y

# Install Python3 
RUN apt-get install -y python3 python3-pip

# Remove EXTERNALLY-MANAGED 
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED || true

# Install Flask 
RUN pip3 install flask

# Set and app 
WORKDIR /app

# Copy  api.py
COPY ./api.py /app/api.py

# run  Flask
CMD ["python3", "api.py"]
