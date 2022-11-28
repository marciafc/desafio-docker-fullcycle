FROM golang:1.19.3-alpine AS build

WORKDIR /app

COPY . .

RUN go mod init desafio-go && \
    go build

#FROM gcr.io/distroless/static-debian11
FROM scratch

WORKDIR /

COPY --from=build /app/desafio-go /desafio-go

ENTRYPOINT ["/desafio-go"]