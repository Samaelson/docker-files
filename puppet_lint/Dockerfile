FROM alpine:edge
RUN echo http://dl-4.alpinelinux.org/alpine/edge/testing/ >> /etc/apk/repositories \
    && apk add --update-cache shadow ruby less bash pylint git \
    && gem install puppet yaml-lint puppet-lint --no-rdoc --no-ri
ENTRYPOINT ["/bin/bash"]
