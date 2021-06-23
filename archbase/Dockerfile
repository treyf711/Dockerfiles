FROM archlinux

RUN pacman -Syu --noconfirm --needed base-devel git sudo 
RUN echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/build
RUN useradd -m builder
USER builder
WORKDIR /home/builder
RUN git clone https://aur.archlinux.org/yay.git
WORKDIR /home/builder/yay
RUN makepkg -si --noconfirm
