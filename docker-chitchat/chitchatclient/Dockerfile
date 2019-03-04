FROM golang 
ADD chitchat/. /go/src/chitchat
WORKDIR /go/src/chitchat
RUN go get github.com/lib/pq
RUN go build 
ENTRYPOINT ./chitchat
EXPOSE 8080

