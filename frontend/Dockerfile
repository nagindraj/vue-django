FROM node:9-alpine

MAINTAINER Nagendra 


RUN mkdir /opt/frontend  
WORKDIR /opt/frontend
ADD . /opt/frontend

#install Yarn
RUN sudo yum install curl
RUN curl -sL https://dl.yarnpkg.com/rpm/yarn.repo -o /etc/yum.repos.d/yarn.repo
RUN sudo yum install yarn

RUN sudo yarn install

EXPOSE 8080

CMD yarn serve


