FROM golang:latest
WORKDIR /go/src/github.com/mchmarny/simple-app/
COPY . .
RUN CGO_ENABLED=0 go build -v -o app

COPY /go/src/github.com/mchmarny/simple-app/app .
ENTRYPOINT ["/app"]
