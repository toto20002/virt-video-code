# FROM alpine:3.14
FROM ubuntu
RUN  

     sudo apt-add-repository ppa:ansible/ansible  && \
     sudo apt update && \
     sudo apt install ansible 

RUN  mkdir /ansible && \
     mkdir -p /etc/ansible && \
     echo 'localhost' > /etc/ansible/hosts

WORKDIR /ansible
COPY ansbile.cfg /ansible/

CMD  [ "ansible-playbook", "--version" ]
