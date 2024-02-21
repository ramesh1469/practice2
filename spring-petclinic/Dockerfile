FROM maven:3.8.5-openjdk-17 as build 
RUN apt update && apt install git & mkdir ssh
COPY ./.ssh/ /ssh/
RUN ssh-keyscan -t rsa github.com >> ./ssh/known_hosts && \
    git clone git@github.com:ramesh1469/practice2.git