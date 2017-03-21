FROM mongo
MAINTAINER davidtnfsh <davidtnfsh@gmail.com> 

# FROM sgoblin/python3.5
RUN sed -i 's/archive.ubuntu.com/mirror.us.leaseweb.net/' /etc/apt/sources.list 
RUN sed -i 's/deb-src/#deb-src/' /etc/apt/sources.list 
RUN apt-get update 
RUN apt-get upgrade -y 
RUN apt-get install -y  build-essential  ca-certificates  gcc  git  libpq-dev  make  pkg-config  python3  python3-dev  python3-pip  aria2 
RUN apt-get autoremove -y 
RUN apt-get clean 

RUN pip3 install -U virtualenv 
# FROM sgoblin/python3.5

# install ifconfig, vim
RUN apt-get install -y net-tools vim

# solve encoding error for chinese
RUN export LANG=C.UTF-8
RUN alias ll='ls -al'

ENTRYPOINT ["/entrypoint.sh"]

CMD ["mongod"]

EXPOSE 8000
