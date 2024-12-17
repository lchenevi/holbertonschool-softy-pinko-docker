# Use the latest version of Ubuntu
FROM ubuntu:latest

# Update and upgrade the system
RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y python3 python3-pip
RUN pip3 install flask

# set working directory
WORKDIR /app
COPY api.py /app/api.py

CMD ["python3", "/app/api.py"]
