FROM cimg/go:1.16

WORKDIR /usr/src/app

ENV PORT=3000
ENV REQUEST_ORIGIN="https://example.com"

COPY . .

RUN go build

RUN go test ./...

CMD ["./server"]
