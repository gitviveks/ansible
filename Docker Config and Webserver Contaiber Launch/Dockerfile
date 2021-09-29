FROM centos:latest
MAINTAINER Vivek Singare <hub.docker.com/u/viveksingare>
LABEL description="SSH enabled centos for Ansible support"

RUN yum install openssh-server -y && \
    yum install passwd -y && \
    ssh-keygen -A && \
    echo vivek | passwd root --stdin
EXPOSE 22
CMD ["/usr/sbin/sshd", "-D"]

