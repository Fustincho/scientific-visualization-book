FROM ubuntu:20.04
ENV DEBIAN_FRONTEND noninteractive
WORKDIR /workspace

RUN apt update \ 
    && apt install make -y\
	&& apt install pkg-config -y\
    && apt install python3 -y\
    && apt install python3-pip -y\
    && apt install git -y\
	&& apt install imagemagick

COPY Dockerfile Makefile requirements.txt /workspace/

RUN make install