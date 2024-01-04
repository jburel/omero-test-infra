ARG OMEROWEB_BASE_IMAGE=openmicroscopy/omero-web:latest
FROM $OMEROWEB_BASE_IMAGE

USER root
RUN dnf clean all
RUN dnf update
RUN yum install -y -q \
    java-11-openjdk \
    git
RUN dnf clean all
USER omero-web
