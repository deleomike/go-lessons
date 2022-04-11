## run .go

```bash
go run hello.go
```

## build .go

```bash
go build hello.go
./hello
```

## build to file name

```bash
go build -o hello_world hello.go
./hello_world
```

# Installing

Go programs are installed via their code repositories, there are no centralized hubs.

```bash
go install github.com/rakyll/hey@latest
hey https://www.golang.org
```

# Formatting

Fixes the imports and formatting

Install formatter
```
go install golang.org/x/tools/cmd/goimports@latest
```
```
goimports -l -w .
```

### Linter

TODO, make these a make file

```
go install golang.org/x/lint/golint@latest
```

```
golint ./...
go vet ./...
```

```
golangci-lint run
```