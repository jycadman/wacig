.DEFAULT_GOAL := build

.PHONY:clean fmt vet build repl
clean:
	go clean -testcache

fmt: clean
	go fmt ./...

vet: fmt
	go vet ./...

build: vet
	go build ./...

repl:
	go build -o monkey .
	./monkey

benchmark: build
	go build -o fibonacci ./benchmark
