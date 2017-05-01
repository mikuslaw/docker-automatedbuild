# A base image build using Debian slim offical image.
FROM debian:7

# Set basic environment variables. Start with defining a linux terminal
ENV TERM xterm
# Disable interactive apt-get
RUN echo 'debconf debconf/frontend select Noninteractive' | debconf-set-selections

# In base image, for testing, run a shell
CMD ["bash"]
