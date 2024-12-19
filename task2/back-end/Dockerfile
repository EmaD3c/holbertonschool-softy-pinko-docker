# image unbuntu la plus recente
FROM ubuntu:22.04

# maj de la liste des paquets APT
RUN apt-get update

# maj des logiciel instaler
RUN apt-get upgrade -y

RUN apt-get install -y python3 python3-pip

RUN rm /usr/lib/python*/EXTERNALLY-MANAGED || true

RUN pip3 install flask

WORKDIR /app

# coopier api.py dans la directorie
COPY ./api.py /app/

# LANCER LAPP FLASK
CMD ["python3", "api.py"]
