# go_micro

This is a project that creates a simple shipping service in order to demonstrate the concept of creating Microservices in Go. This is a learning exercise and I am indebted to the author of [this](https://ewanvalentine.io/microservices-in-golang-part-1/) blog series.

# Set up

Ensure that the GOPATH is set.

~~~ text
export GOPATH=$HOME/go
export PATH=$PATH:$GOPATH/bin
mkdir -p $GOPATH/src/github.com/user
~~~

Install dependencies:

~~~ text
go get -u google.golang.org/grpc                                                                                                                                 
go get -u github.com/golang/protobuf/protoc-gen-go
~~~

In addition, I had to install protobuf:

~~~ text
brew install protobuf
~~~

# Usage

In a terminal, change to the consignment-service directory and run:

~~~ text
go run main.go
~~~

From another terminal, change to the consignment-cli directory and run:

~~~ text
go run cli.go
~~~

