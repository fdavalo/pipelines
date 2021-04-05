FROM registry.access.redhat.com/ubi7/ubi  

RUN curl https://github.com/kubevirt/kubevirt/releases/download/v0.39.0/virtctl-v0.39.0-linux-amd64 -L -o virtctl && \
    mv virtctl /usr/bin && chmod +x /usr/bin/virtctl 

USER 1001

ENTRYPOINT ["/usr/bin/virtctl"]
