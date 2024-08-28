# Use the latest version of Ubuntu as the base image
FROM ubuntu:latest

# Update the list of available packages
RUN apt-get update

# Upgrade the installed packages
RUN apt-get upgrade -y

# Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# Remove EXTERNALLY-MANAGED file if it exists
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED || true

# Install Flask and flask-cors using pip3
RUN pip3 install flask flask-cors

# Set /app as the working directory
WORKDIR /app

# Copy the api.py file to /app directory inside the Docker image
COPY ./api.py /app/api.py

# Command to run the Flask application
CMD ["python3", "api.py"]
