FROM golang:1.27

EXPOSE 8080

WORKDIR /usr/src/app

RUN apt update && apt install -y golang-go

COPY . .

RUN go build

RUN go test ./...

CMD ["./server"]


