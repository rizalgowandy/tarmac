## Makefile for Go example for Tarmac WASM functions

build:
	## Run TinyGo build via Docker because its easier
	docker run -v `pwd`/:/build -w /build tinygo/tinygo:0.18.0 tinygo build -o /build/tarmac.wasm -target wasi /build/main.go

docker-compose:
	docker compose up

run: build docker-compose
