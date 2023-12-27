# graphql-go [![Sourcegraph](https://sourcegraph.com/github.com/graph-gophers/graphql-go/-/badge.svg)](https://sourcegraph.com/github.com/graph-gophers/graphql-go?badge) [![Build Status](https://graph-gophers.semaphoreci.com/badges/graphql-go/branches/master.svg?style=shields)](https://graph-gophers.semaphoreci.com/projects/graphql-go) [![Go Report](https://goreportcard.com/badge/github.com/graph-gophers/graphql-go)](https://goreportcard.com/report/github.com/graph-gophers/graphql-go) [![GoDoc](https://godoc.org/github.com/graph-gophers/graphql-go?status.svg)](https://godoc.org/github.com/graph-gophers/graphql-go)

<p align="center"><img src="docs/img/Graphql.png" width="300"></p>

The goal of this project is to provide full support of the [October 2021 GraphQL specification](https://spec.graphql.org/October2021/) with a set of idiomatic, easy to use Go packages.

This is under development (`internal` APIs are almost certainly subject to change), this library is safe for production use.

## Features

- minimal API
- support for `context.Context`
- support for the `OpenTelemetry` and `OpenTracing` standards
- schema type-checking against resolvers
- resolvers are matched to the schema based on method sets (can resolve a GraphQL schema with a Go interface or Go struct).
- handles panics in resolvers
- parallel execution of resolvers
- subscriptions
  - [sample WS transport](https://github.com/graph-gophers/graphql-transport-ws)
- directive visitors on fields (the API is subject to change in future versions)

