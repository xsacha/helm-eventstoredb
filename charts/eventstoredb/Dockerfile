FROM eventstore/eventstore:23.6.0-bionic as base

USER eventstore

COPY certs/ca/ca.crt /etc/eventstore/certs/ca/ca.crt
COPY certs/node1/node.crt /etc/eventstore/certs/node.crt
COPY certs/node1/node.key /etc/eventstore/certs/node.key
COPY eventstore.conf /etc/eventstore/eventstore.conf

WORKDIR /opt/eventstore

ENV EVENTSTORE_EXT_HOST_ADVERTISE_AS=localhost
ENV EVENTSTORE_INT_HOST_ADVERTISE_AS=localhost

