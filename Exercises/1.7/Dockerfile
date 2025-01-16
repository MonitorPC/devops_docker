FROM ubuntu:22.04

WORKDIR /usr/src/app

COPY . .

RUN apt update && apt install curl -y

RUN chmod +x script.sh

CMD ["sh", "script.sh"]

