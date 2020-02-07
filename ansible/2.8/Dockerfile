FROM ubuntu:18.10

RUN apt-get update && apt-get install -y software-properties-common \
    && apt-add-repository --yes --update ppa:ansible/ansible \
    && apt-get install -y ansible=2.8.2-1ppa~cosmic vim rsync python-pip python3-pip git iputils-ping \
    && rm -rf /var/lib/apt/lists/* \
    && python -m pip install --upgrade pip netaddr \
    && python3 -m pip install --upgrade pip netaddr

WORKDIR /opt/ansible