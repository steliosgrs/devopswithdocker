# Start from the alpine image
FROM golang:1.16

WORKDIR /path/golang/app/

COPY ./example-backend .

RUN go build

RUN go test .

ENV REQUEST_ORIGIN=https://example.com

EXPOSE 8080

ENTRYPOINT [ "./server" ] 