FROM golang:1.20.1-alpine3.17

COPY main.go .

RUN go build main.go

EXPOSE 8080

CMD [ "./main" ]
