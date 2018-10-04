## TCP Server

*This is a TCP Server and distributed app example in Elixir*

* First install dependencies with `mix deps.get`
* Run tests with `mix test`

## Running TCP Server on the console.

To run this open a console and start the server.

```
$ iex -S mix
iex> App.Server.start(4001)
```

The ```-S mix``` options will load your project into the current session.

Open another console and connect using telnet.

```
$ telnet 127.0.0.1 4001
Trying 127.0.0.1...
Connected to localhost.
Escape character is '^]'.
hello
hello
is it me
is it me
you are looking for?
you are looking for?
```

My particular telnet client can be exited by typing ctrl + ], typing quit, and pressing Enter, but your client may require different steps.

## Distributed HttpServer

Running the command below automatically starts HttpServer too.

```
$ iex -S mix
```

Now you can visit [`localhost:8888`](http://localhost:8888) from your browser.

Use /kaboom to raise an exception and start a new process.
http://localhost:8888/kaboom
