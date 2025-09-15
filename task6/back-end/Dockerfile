# gets latest version of Ubuntu
FROM ubuntu:latest

# Set non-interactive frontend at the beginning
ENV DEBIAN_FRONTEND=noninteractive

# updates APT package index
RUN apt-get update

# upgrades currently installed software
RUN apt-get upgrade -y

# install python3, pip3 and Flask
RUN apt-get install python3 && \
apt-get install python3-pip

RUN pip install --break-system-packages flask flask-cors

RUN mkdir -p /app

COPY api.py /app/

RUN cd /app && \
    chmod u+x api.py

WORKDIR /app

CMD python3 api.py
