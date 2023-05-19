FROM golang:1.16

WORKDIR /usr/src/app

COPY . .

RUN go build -o server

RUN go test ./...

# These are default values
ENV PORT=8080
ENV REQUEST_ORIGIN=https://example.com

EXPOSE 8080

CMD ["./server"]


# Command to build and run:
# docker build . -t example_back && docker run -p 127.0.0.1:8080:8080 example_back
