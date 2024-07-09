.DEFAULT_GOAL := build

.PHONY:fmt vet build repl clean
fmt:
	go fmt ./...

vet: fmt
	go vet ./...

build: vet
	go build ./...

test-define:
	go test -run TestDefine ./compiler

test-resolve:
	go test -run TestResolveGlobal ./compiler

repl:
	go build -o monkey .
	./monkey

clean:
	go clean -testcache
