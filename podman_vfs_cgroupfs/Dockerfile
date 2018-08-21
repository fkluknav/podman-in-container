FROM registry.fedoraproject.org/fedora

LABEL maintainer="fkluknav@redhat.com"

RUN dnf -y install podman && dnf clean all

VOLUME /var/lib/containers

LABEL usage="docker run -it --privileged podman <command>. You get podman with vfs handling storage and cgroupfs handling cgroups - options you probably want in a container. You might want to mount a volume for the storage into /var/lib/containers."

ENTRYPOINT ["podman", "--storage-driver=vfs", "--cgroup-manager=cgroupfs"]
