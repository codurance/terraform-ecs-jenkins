FROM jenkins/jenkins:2.100

COPY plugins.txt /usr/share/jenkins/plugins.txt

RUN apt-get update -y && apt-get install -y zip awscli jq
RUN /usr/local/bin/plugins.sh /usr/share/jenkins/plugins.txt
