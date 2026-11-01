FROM docker.io/library/python:3.16.0a1-slim@sha256:b76a57911c515b9ce22946525c73561bfdf4100c3df36e48115dae97b02447b4

COPY docker/latest/requirements.txt /var/tmp/build/

RUN \
    pip install --no-deps -r /var/tmp/build/requirements.txt && \
    rdfpipe --version

ENTRYPOINT [ ]
