FROM python:3
MAINTAINER Jonathan Rodriguez "jrodrig2@uoregon.edu"
RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential
COPY . /vocab
WORKDIR /vocab
RUN pip install -r requirements.txt
ENTRYPOINT ["python3"]
CMD ["flask_vocab.py"]
