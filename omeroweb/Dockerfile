ARG OMEROWEB_BASE_IMAGE=openmicroscopy/omero-web:latest
FROM $OMEROWEB_BASE_IMAGE

USER root
RUN dnf clean all && rm -rf /var/cache/dnf/*pgdg*/
RUN dng check-updates
RUN yum install -y -q \
    java-11-openjdk \
    git
RUN yum clean metadata && yum clean all
USER omero-web
