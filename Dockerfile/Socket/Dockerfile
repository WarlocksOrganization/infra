FROM ubuntu:20.04
RUN apt-get -qq update \
&& apt-get -qq install -y g++ cmake wget unzip python3 \
&& apt-get clean

EXPOSE 8080
ENTRYPOINT ["/bin/bash"]
