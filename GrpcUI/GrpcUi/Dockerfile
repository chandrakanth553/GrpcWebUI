FROM golang:1.14

WORKDIR /go/src/app
COPY . .

RUN go get github.com/fullstorydev/grpcui/...
RUN go install github.com/fullstorydev/grpcui/cmd/grpcui

CMD ["grpcui", "127.0.0.1:5001"]