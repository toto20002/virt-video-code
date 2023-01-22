# FROM alpine:3.14
FROM ubuntu
RUN  apt-add-repository ppa:ansible/ansible  && \
     apt update && \
     apt install ansible

RUN  mkdir /ansible && \
     mkdir -p /etc/ansible && \
     echo 'localhost' > /etc/ansible/hosts

WORKDIR /ansible
COPY ansbile.cfg /ansible/

CMD  [ "ansible-playbook", "--version" ]
