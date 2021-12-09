from archlinux

# Just enough to run docker-compose inside docker from archlinux. bind mount the docker socket to the container to actually get things done.

VOLUME ["/compose"]
RUN pacman -Syyu --noconfirm docker-compose
