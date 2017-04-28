FROM jmikucki/debian-base

RUN apt-get update -q \
    && DEBIAN_FRONTEND=noninteractive apt-get install -yq --no-install-recommends \
    curl openssh-server ca-certificates postfix wget
    
# RUN ["wget", "https://packages.gitlab.com/gitlab/gitlab-ce/packages/debian/wheezy/gitlab-ce_9.1.1-ce.0_amd64.deb/download", "-O", "/tmp/gitlab.deb"]
# RUN ["dpkg", "-i", "/tmp/gitlab.deb"]

RUN wget https://packages.gitlab.com/install/repositories/gitlab/gitlab-ce/script.deb.sh
RUN bash script.deb.sh
RUN apt-get install gitlab-ce
#RUN gitlab-ctl reconfigure

CMD ["/bin/bash"]
