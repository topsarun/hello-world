FROM python:3-alpine
WORKDIR /usr/src/app
EXPOSE 8000

ARG HELLO_NAME=NONE
ENV HELLO_NAME=$HELLO_NAME

COPY requirements.txt .
RUN pip install -qr requirements.txt
COPY server.py .
CMD ["python3", "./server.py"]