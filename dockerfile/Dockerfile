FROM ubuntu:22.04
LABEL maintainer="Sander <mail@sandervanvugt.nl>"

RUN apt-get update && \
    apt-get install -y nmap iproute2 && \
    apt-get clean

ENTRYPOINT ["/usr/bin/nmap"]
CMD ["-sn", "172.17.0.0/24"]
