FROM ubuntu:14.10

MAINTAINER Walery Strauch

ENV LANG en_US.UTF-8

RUN apt-get update
RUN apt-get install -y -q python-dev python-pip python-lxml libcairo2 libpango1.0-0 libgdk-pixbuf2.0-0 libffi-dev shared-mime-info
RUN pip install WeasyPrint

CMD weasyprint

