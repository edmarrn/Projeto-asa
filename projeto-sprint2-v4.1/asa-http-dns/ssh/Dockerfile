FROM ubuntu:latest

RUN apt update

RUN apt upgrade -y

RUN apt install openssh-server openssh-client -y

# add user
RUn useradd -m redes

RUN echo "redes:redes0123" | chpasswd

CMD ["service", "ssh", "start", "-D"]