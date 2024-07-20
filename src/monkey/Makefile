.DEFAULT_GOAL := build

.PHONY:fmt vet build repl clean
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
