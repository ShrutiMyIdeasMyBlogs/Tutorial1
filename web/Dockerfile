FROM python:3.7-slim

#RUN apt-get update && \
#  apt-get install -y software-properties-common && \
#  add-apt-repository ppa:deadsnakes/ppa
#RUN apt-get update
#FROM ubuntu:16.04
#
#RUN apt-get install -y build-essential python3.6 python3.6-dev python3-pip python3.6-venv
#RUN apt-get install -y git
#RUN python3.6 -m pip install pip --upgrade
#RUN python3.6 -m pip install wheel
#

WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt

COPY . .

CMD ["python3","main.py"]
