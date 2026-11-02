FROM golang:1.22.1

WORKDIR /app
COPY go.mod go.sum imager.go ./
COPY cli ./cli
COPY script ./script
RUN go build -o image-builder ./cli

ENTRYPOINT ["/app/image-builder"]
