# Tokio Mini Redis

This is a example of how to use tokio for tcp connections and async processing with an database

## How to run

### Server

The server listens for messages from the client

If it is a `SET` request, it registers the value to the db

If it is a `GET` request, it returns the value from the db

```shell
cargo run --bin server
```
### Client

It sends two hard-coded messages to the server

```shell
cargo run --bin client
```