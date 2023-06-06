
# mac环境设置
go env -w CGO_ENABLED=0 GOOS=linux   GOARCH=amd64
go env -w CGO_ENABLED=0 GOOS=windows GOARCH=amd64

## linux
go env -w CGO_ENABLED=0 GOOS=darwin   GOARCH=amd64
go env -w CGO_ENABLED=0 GOOS=windows GOARCH=amd64

## windows
go env -w CGO_ENABLED=0 GOOS=darwin3   GOARCH=amd64
go env -w CGO_ENABLED=0 GOOS=linux GOARCH=amd64


## go设置源

## go模块
go mod init
go mod download







