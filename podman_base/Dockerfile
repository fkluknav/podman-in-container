FROM registry.fedoraproject.org/fedora

LABEL maintainer="fkluknav@redhat.com"

RUN dnf -y install podman skopeo && dnf clean all

VOLUME /var/lib/containers

LABEL usage="docker run --privileged podman. You get a shell with podman, buildah, skopeo and associated tools available. You might want to mount a volume for the storage into /var/lib/containers.
