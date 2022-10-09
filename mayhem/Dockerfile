FROM golang:1.18 as builder

ADD . /celestia-app
WORKDIR /celestia-app
RUN go mod tidy
RUN go build ./cmd/celestia-appd

# Package Stage
# FROM debian:bookworm-slim
# COPY --from=builder /celestia-app/celestia-appd /
