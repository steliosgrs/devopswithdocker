# Start from the alpine image
FROM golang:1.16

WORKDIR /path/golang/app/

COPY ./example-backend .

RUN go build

RUN go test .

ENV REQUEST_ORIGIN=http://localhost:5000

ENV PORT=9000

EXPOSE 9000

ENTRYPOINT [ "./server" ] 