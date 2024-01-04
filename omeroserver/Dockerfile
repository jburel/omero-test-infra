ARG OMEROSERVER_BASE_IMAGE=openmicroscopy/omero-server:latest
FROM $OMEROSERVER_BASE_IMAGE

USER root
#RUN dnf clean all && dnf update
RUN yum clean metadata && yum clean all &&  yum update
RUN yum install -y -q --nogpgcheck\
    git
RUN yum clean metadata && yum clean all
USER omero-server
