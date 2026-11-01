FROM docker.io/library/python:3.16.0a1-slim@sha256:b76a57911c515b9ce22946525c73561bfdf4100c3df36e48115dae97b02447b4

# This file is generated from docker:unstable in Taskfile.yml
COPY var/requirements.txt /var/tmp/build/

RUN \
    pip install -r /var/tmp/build/requirements.txt

COPY dist/*.whl /var/tmp/build/

RUN \
    pip install --no-deps /var/tmp/build/*.whl && \
    rdfpipe --version

ENTRYPOINT [ ]
