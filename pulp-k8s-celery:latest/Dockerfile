FROM mhrivnak/pulp-k8s-base

ADD run.sh /run.sh

USER root

RUN dnf install -y socat && dnf clean all

# Usage: /run.sh worker|beat|resource_manager
ENTRYPOINT ["/run.sh"]
