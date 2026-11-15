FROM docker.io/library/python:3.16.0a2-slim@sha256:b743a8ab2708d630f1c1c008ef5c99d4b635ec16bb2012284f731d9957a14a1c

COPY docker/latest/requirements.txt /var/tmp/build/

RUN \
    pip install --no-deps -r /var/tmp/build/requirements.txt && \
    rdfpipe --version

ENTRYPOINT [ ]
