### `./material-applications/example-frontend/Dockerfile`

```
FROM node:16

WORKDIR /usr/src/app

EXPOSE 5000

COPY . .

RUN npm install

RUN npm install -g serve

RUN REACT_APP_BACKEND_URL="http://localhost:8080" npm run build

CMD ["serve", "-s", "-p", "5000", "build"]
```

### `./material-applications/example-backend/Dockerfile`

```
FROM cimg/go:1.16

WORKDIR /usr/src/app

EXPOSE 8080

ENV PORT=8080
ENV REQUEST_ORIGIN="http://localhost:5000"
ENV REDIS_HOST="redis"

COPY . .

RUN go build

RUN go test ./...

CMD ["./server"]
```

### Command to start 

`docker compose up --build`
