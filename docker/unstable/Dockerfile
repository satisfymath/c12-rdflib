FROM docker.io/library/python:3.16.0a2-slim@sha256:b743a8ab2708d630f1c1c008ef5c99d4b635ec16bb2012284f731d9957a14a1c

# This file is generated from docker:unstable in Taskfile.yml
COPY var/requirements.txt /var/tmp/build/

RUN \
    pip install -r /var/tmp/build/requirements.txt

COPY dist/*.whl /var/tmp/build/

RUN \
    pip install --no-deps /var/tmp/build/*.whl && \
    rdfpipe --version

ENTRYPOINT [ ]
