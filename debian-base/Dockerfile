# A base image build using Debian slim offical image.
FROM debian:jessie-slim

# Set basic environment variables. Start with defining a linux terminal
ENV TERM Linux
# Disable interactive apt-get
RUN echo 'debconf debconf/frontend select Noninteractive' | debconf-set-selections

# In base image, for testing, run a shell
CMD ["bash"]
