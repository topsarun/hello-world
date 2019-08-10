FROM python:3-alpine
WORKDIR /usr/src/app
EXPOSE 8000

ARG HELLO-NAME=NONE
ENV HELLO-NAME=$HELLO-NAME

COPY requirements.txt .
RUN pip install -qr requirements.txt
COPY server.py .
CMD ["python3", "./server.py"]