FROM docker.io/python:3.5
MAINTAINER wmp <wmp@beyondsoft.com>
RUN rm -rf /etc/apt/sources.list
ADD sources.list /etc/apt/
ADD nginx.list /etc/sources.list.d/
ADD nginx_signing.key /
RUN apt-key add /nginx_signing.key
RUN apt-get update
RUN apt-get install -y vim net-tools nginx htop
