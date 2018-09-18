# go-graphql

## Prerequistes
- Prisma cli version 1.17 beta installed
- Go installed
- gqlgen installed

## Getting started

```sh
~ $ git clone https://github.com/Sach97/prisma-go-todo/edit/master/README.md 
~ $ ln -s ~/prisma-go-todo ~/go/src/prisma-go-todo (convenient but not required see https://codebasecamp.com/2017/04/25/Project-Structure-Go.1/ for an explanation of symlinks )
~ $ cd prisma-go-todo
prisma-go-todo $ docker-compose up -d (kill your docker container running with you have errors)
prisma-go-todo $ cd prisma
prisma $ prisma deploy
prisma $ cd ..
prisma-go-todo $ go run server/*.go # Install missing dependencies then rerun this command
```

## Development Workflow

- Modify your datamodel.prisma
- prisma deploy
- Modify your schema.graphql
- gqlgen -v (must be executed in your GOPATH)
- Modify your generated tmp/resolver with the prisma generated types
- run server

## TODOs
- [ ] Auth and permissions
