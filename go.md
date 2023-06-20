
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

## go 大小写敏感

## json
go通过首字母大小写确定当前字段或方法是否公开
在序列化struct为json时，若字段小写则序列化有问题


## goLang
unresolve dependency

勾选
file -> settings -> Go Modules -> Enable Go modules integration






