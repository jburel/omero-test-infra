ARG OMEROWEB_BASE_IMAGE=openmicroscopy/omero-web:latest
FROM $OMEROWEB_BASE_IMAGE

USER root
#RUN dnf clean all && dnf update
RUN yum clean metadata && yum clean all && yum update
RUN yum install -y -q \
    java-11-openjdk \
    git
RUN yum clean metadata && yum clean all
USER omero-web
