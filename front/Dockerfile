# BUILD
FROM golang:alpine as builder

COPY dispatcher.go .
RUN go build dispatcher.go

# RUN
FROM alpine:3.16.0

EXPOSE 80

COPY --from=builder /go/dispatcher /
COPY static /static/

CMD ["/dispatcher"]
