ARG OMEROSERVER_BASE_IMAGE=openmicroscopy/omero-server:latest
FROM $OMEROSERVER_BASE_IMAGE

USER root
RUN dnf clean all && rm -rf /var/cache/dnf/*pgdg*/
RUN dnf check-updates
RUN yum install -y -q --nogpgcheck\
    git && \
    dnf clean all
USER omero-server
