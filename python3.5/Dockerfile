# Base python 3.5 build, inspired by 
# https://github.com/crosbymichael/python-docker/blob/master/Dockerfile 
FROM sgoblin/python3.5
MAINTAINER davidtnfsh <davidtnfsh@gmail.com> 

# install ifconfig
RUN apt-get update
RUN apt-get install -y net-tools vim wget

# solve encoding error for chinese
ENV LANG=C.UTF-8

# add ll in alias
RUN export alias ll='ls -al'

CMD [] 

EXPOSE 8000
