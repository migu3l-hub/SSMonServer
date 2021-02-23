FROM tsl0922/ttyd:1.6.0

RUN apt-get update -y && apt-get upgrade -y && apt-get -y clean
RUN apt-get install net-tools -y
RUN apt-get install nano -y
RUN apt-get install ssh -y
RUN apt-get install iputils-ping -y


CMD ttyd -c usrttyd:pwdttyd -p 7681 bash

EXPOSE 7681

#docker run --name mitty -d -p 8888:7681 monitor_tty
