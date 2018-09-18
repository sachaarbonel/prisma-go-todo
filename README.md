# go-graphql

## Prerequistes
- Go installed
- Symlinks (not required but convenient) 
## Getting started

```sh
~ $ git clone https://github.com/Sach97/prisma-go-todo/edit/master/README.md 
~ $ cd prisma-go-todo
prisma-go-todo $ docker-compose up
prisma-go-todo $ cd prisma
prisma $ prisma deploy
prisma $ cd ..
prisma-go-todo $ go run server/*.go # Install missing dependencies then rerun this command
```

## Development Workflow

- Modify your prisma.datamodel
- prisma deploy
- Modify your schema.graphql
- gqlgen -v (must be executed in your GOPATH)
- Modify your generated tmp/resolver with the prisma generated types
- run server
