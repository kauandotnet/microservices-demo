# BUILD STAGE
FROM golang:1.13.7-alpine as builder
RUN apk add --no-cache ca-certificates git
WORKDIR /caddy
COPY . .
RUN go get ./... && \
    go install


# FINAL STAGE
FROM alpine:3.11
COPY --from=builder /go/bin/caddy /bin/caddy
RUN apk add --no-cache ca-certificates
WORKDIR /www

EXPOSE 80 443
ENTRYPOINT [ "caddy" ]

# USER nobody
# EXPOSE 8080 8443
# ENTRYPOINT [ "caddy", "-http-port", "8080", "-https-port", "8443" ]
