FROM ubuntu:14.04.3
ENV DEBIAN_FRONTEND noninteractive

# update apt-package-index
RUN apt-get install -y curl
RUN apt-get -o Debug::Acquire::http=true  update && apt-get install -y build-essential python-dev python-setuptools nginx-extras libgnutls-dev supervisor

RUN easy_install pip && pip install boto uwsgi
ENV LC_ALL C.UTF-8
