### Crud API with GRPC and Golang
<hr>
<br>
<strong>Run the commands to generate .proto files</strong>
<br>
$ export PATH="$PATH:$(go env GOPATH)/bin"
<br>
<br>
$ protoc --go_out=. --go_opt=paths=source_relative \
  --go-grpc_out=. --go-grpc_opt=paths=source_relative \
  protos/moviesapp.proto
<br>
<br>
$go mod tidy

<br>
<hr>
 <strong>Running the server and client</strong>
 <br>
 <br>
$ go run cmd/server/*.go

<br>
<br>
<strong>open another terminal and run:</strong>
<br>
<br>
$ go run cmd/client/*.go
