FROM alpine
RUN apk add --update --no-cache curl jq py3-configobj py3-pip py3-setuptools python3 python3-dev
    
RUN apk --purge -v del py-pip
CMD tail -f /dev/null