FROM archbase

USER root
RUN pacman -S --needed --noconfirm go

USER builder
WORKDIR /home/builder
RUN git clone https://github.com/mop-tracker/mop
WORKDIR /home/builder/mop
RUN go build ./cmd/mop
CMD /home/builder/mop/mop
