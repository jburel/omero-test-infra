ARG OMEROSERVER_BASE_IMAGE=openmicroscopy/omero-server:latest
FROM $OMEROSERVER_BASE_IMAGE

USER root
RUN dnf clean all && rm -r /var/cache/dnf  && dnf upgrade -y && dnf update -y 
RUN yum install -y -q \
    git && \
    dnf clean all
USER omero-server
