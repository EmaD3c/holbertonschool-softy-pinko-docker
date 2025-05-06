FROM ubuntu:25.04

RUN apt-get update

RUN apt-get upgrade -y

CMD echo "Hello, World!"

RUN apt-get install -y python3 python3-pip

RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

RUN pip3 install flask

WORKDIR /app

COPY /api.py /app/

CMD ["python3", "api.py"]
