ARG OMEROWEB_BASE_IMAGE=openmicroscopy/omero-web:latest
FROM $OMEROWEB_BASE_IMAGE

USER root
RUN yum install -y -q \
    java-11-openjdk \
    git
RUN dnf clean all
USER omero-web
