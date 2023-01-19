Jan 2023

 --> brew install protobuf
To install Go specific gRPC dependencies:

go install google.golang.org/protobuf/cmd/protoc-gen-go@latest
go install oogle.golang.org/grpc/cmd/protoc-gen-go-grpc@latest

--> Check the gopath if you have eror


To generate the .pb.go and _grpc.pb.go

protoc --proto_path=proto proto/*.proto --go_out=. --go-grpc_out=.