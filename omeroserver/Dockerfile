ARG OMEROSERVER_BASE_IMAGE=openmicroscopy/omero-server:latest
FROM $OMEROSERVER_BASE_IMAGE

USER root
RUN mv /etc/yum.repos.d/pgdg-redhat-all.repo /tmp
RUN yum install -y -q \
    git && \
    dnf clean all
USER omero-server
