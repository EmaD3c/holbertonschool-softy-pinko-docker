# # image unbuntu la plus recente
FROM ubuntu:22.04

# maj de la liste des paquets APT / maj des logiciel instaler
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y --no-install-recommends python3 python3-pip && \
    apt-get clean

# suppression de la restriction(si nécessaire)
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED || true

RUN pip3 install flask flask-cors

WORKDIR /app

# coopier api.py dans la directorie
COPY ./api.py /app/

# LANCER LAPP FLASK
CMD ["python3", "api.py"]
