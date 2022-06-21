FROM node:16.15.1-alpine3.15
# WORKDIR /usr/src
EXPOSE 4000 5001 9000 8080 8085 5000 4200 3333
RUN apk update \
  && apk add --no-cache git openssh openjdk8 bash \
  && yarn global add @angular/cli @compodoc/compodoc ts-node typescript jest nx
RUN yarn
ENV JAVA_HOME /usr/lib/jvm/java-1.8-openjdk
ENV PATH $PATH:$JAVA_HOME/bin