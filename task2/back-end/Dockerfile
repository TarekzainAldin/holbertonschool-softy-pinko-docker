
#  version of Ubuntu 
FROM ubuntu:latest

# Update  packages
RUN apt-get update

#installed packages
RUN apt-get upgrade -y

# Install Python3 
RUN apt-get install -y python3 python3-pip

# Remove EXTERNALLY-MANAGED
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED || true

# Install Flask 
RUN pip3 install flask

# Set /app 
WORKDIR /app

# Copy 
COPY ./api.py /app/api.py

# run the Flask 
CMD ["python3", "api.py"]
