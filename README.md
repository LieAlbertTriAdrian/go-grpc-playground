# go-grpc-playground
Playground for experimenting with gRPC in Go

* [go-grpc-playground](#go-grpc-playground)
	* [Setup](#setup)
	* [Onboarding](#onboarding)
		* [Run](#run)
	* [TODO:](#todo)

## Setup
* [Go](https://golang.org/)
* [Proto Compiler](https://developers.google.com/protocol-buffers/docs/downloads)
* [Proto Go Package](https://github.com/golang/protobuf/proto)
* [Proto Go Generator Go Package](https://github.com/golang/protobuf/protoc-gen-go)

## Onboarding

### Run
* Compile the protobuf file first by going into root folder and running
```
protoc -I customer/ customer/customer.proto --go_out=plugins=grpc:customer
```
* File `customer.pb.go` will be created under `customer` folder
* Run the rpc server by going into server folder and run
```
go run main.go
```
* Run the rpc client by going into client folder and run
```
go run main.go
```

## TODO:
* Add tracer
* Add streaming example
* Add contract generation
