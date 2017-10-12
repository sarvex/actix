# Chat example


## Server

Chat server listens for incoming tcp connections. Server can access several types of message:

  * `\list` - list all available rooms
  * `\join name` - join room, if room does not exist, create new one
  * `some message` - just string, send messsage to all peers in same room
  
To start server use command: `cargo run --bin server`

## Client

Client connects to server. Reads input from stdin and sends to server.

To run client use command: `cargo run --bin client`