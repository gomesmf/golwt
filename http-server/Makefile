bin:
	-mkdir -p bin

build_cli: bin
	go build -o bin/poker-cli cmd/cli/main.go

build_web: bin
	go build -o bin/poker-web cmd/webserver/main.go

build: build_cli build_web

clean:
	-rm -rf bin
	-rm game.db.json

run_cli:
	./bin/poker-cli

run_web:
	./bin/poker-web