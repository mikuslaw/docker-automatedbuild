FROM jmikucki/debian-base

RUN apt-get update -q \
    && DEBIAN_FRONTEND=noninteractive apt-get install -yq --no-install-recommends \
    curl openssh-server ca-certificates postfix
    
ADD ["https://packages.gitlab.com/gitlab/gitlab-ce/packages/debian/wheezy/gitlab-ce_9.1.1-ce.0_amd64.deb/download", "/temp/"]
RUN ["dpkg", "-i gitlab*"]

CMD ["bash"]
