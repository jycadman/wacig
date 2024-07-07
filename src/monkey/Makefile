.DEFAULT_GOAL := build

.PHONY:fmt vet build repl clean
fmt:
	go fmt ./...

vet: fmt
	go vet ./...

build: vet
	go build ./...

repl:
	go build -o monkey .
	./monkey

clean:
	go clean -testcache
