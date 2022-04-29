FROM alpine
RUN apt add --no-cache curl wget busybox-extras netcat-openbsd python py-pip bash && \
    pip install awscli
RUN apt --purge -v del py-pip
CMD tail -f /dev/null