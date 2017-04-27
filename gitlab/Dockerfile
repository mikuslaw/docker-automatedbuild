FROM jmikucki/debian-base

RUN apt-get update \
    && apt-get install curl openssh-server ca-certificates postfix
    
RUN curl -s https://packages.gitlab.com/install/repositories/gitlab/gitlab-ce/script.deb.sh
RUN sudo bash script.deb.sh
RUN sudo apt-get install gitlab-ce=9.1.1-ce.0

CMD["bash"]
