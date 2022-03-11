ARG OMEROWEB_BASE_IMAGE=openmicroscopy/omero-web:latest
FROM $OMEROWEB_BASE_IMAGE

USER root
RUN /opt/omero/web/venv3/bin/pip uninstall omero-web
RUN yum install -y -q \
    java-11-openjdk \
    git && \
    rm -rf /var/cache/yum
USER omero-web
