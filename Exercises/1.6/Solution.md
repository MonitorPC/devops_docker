`docker run -it devopsdockeruh/pull_exercise`

`docker exec eloquent_lumiere cat Dockerfile`

The output is:
*
FROM node:alpine

WORKDIR /usr/app
COPY . .

CMD ["node", "index.js"]
*

`docker exec eloquent_lumiere cat index.js | less`

In this file i found:
*const KNOWN_INPUTS = {
  "exit": close('exit'),
  "close": close('close'),
  "quit": close('quit'),
  "": close('empty'),
  "help": help(),
  "basics": victory()
}*

***basics*** is the password
