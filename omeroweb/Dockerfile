ARG OMEROWEB_BASE_IMAGE=openmicroscopy/omero-web:latest
FROM $OMEROWEB_BASE_IMAGE

USER root
RUN dnf install -y -q \
    java-11-openjdk \
    git && \
    dnf clean all

RUN /opt/omero/web/venv3/bin/pip install omero-web-zarr
ADD webapps.omero /opt/omero/web/config/

USER omero-web
