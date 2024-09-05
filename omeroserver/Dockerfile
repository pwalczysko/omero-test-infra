ARG OMEROSERVER_BASE_IMAGE=openmicroscopy/omero-server:latest
FROM $OMEROSERVER_BASE_IMAGE

USER root
RUN dnf clean all
    rm -rf /var/cache/dnf/*pgdg*
    dnf install -y -q \
    git && \
    dnf clean all
USER omero-server
