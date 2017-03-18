# Base python 3.5 build, inspired by 
# https://github.com/crosbymichael/python-docker/blob/master/Dockerfile 
FROM sgoblin/python3.5
MAINTAINER davidtnfsh <davidtnfsh@gmail.com> 

# install ifconfig
RUN apt-get install -y net-tools vim

# solve encoding error for chinese
RUN export LANG=C.UTF-8

CMD [] 

ENTRYPOINT ["/bin/bash"]