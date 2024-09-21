FROM golang:1.18

WORKDIR /go/src/app

COPY go.mod . 
COPY go.sum .
COPY main.go .

RUN go mod download
RUN go install

CMD ["dispatch"]
