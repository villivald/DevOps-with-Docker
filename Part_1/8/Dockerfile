FROM ubuntu:18.04
COPY curler.sh .
RUN chmod +x curler.sh
RUN apt update
RUN apt upgrade -y
RUN apt install -y curl
CMD ./curler.sh

