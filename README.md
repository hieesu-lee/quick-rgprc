# Quick gRPC Practice
> Protocol Buffer  
> gRPC  

## Prerequsites
- Go
- Protocol buffer
- Go plugins for the protocol compiler
    - 1. Install the protocol compiler plugins for Go using the following command:
    ```bash
    go install google.golang.org/protobuf/cmd/protoc-gen-go@v1.26
    go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@v1.1
    ```
    - 2. Update `PATH` so that the `protoc` compiler can find the plugins:
    ```bash
    export PATH="$PATH:$(go env GOPATH)/bin"
    ```

## Flow
- Define a service in a `.proto` file
- Generate server and client code using the protocol buffer compiler
- Use the Go gRPC API to write a simple client and server for your service