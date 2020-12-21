# Introduction

Hello!

Aero is a new programming language built on top of Erlang, aiming to give the
same concurrent properties of Erlang, but with statically typed guarantees.

> **Note**:
>
> **Aero is still very much in development and lots of features either are not
> currently implemented or use a naive implementation. Don't rely on parts of
> the language being stable.**

You can check out the source on GitHub at
[aerolang/aero](https://github.com/aerolang/aero). As features land, more and
more things will be added to this site!

## A Glimpse

For a quick look into Aero, here's a simple "Hello, World!" program.

```aero
// hello.aero
pub func main() ->> () {
  log "Hello, World!"
}
```

This can be compiled and run as an Erlang Escript:

```sh
$ aero compile hello.aero --escript && ./out/bin/hello
Hello, World!
```

See the [Aero source repository](https://github.com/aerolang/aero) on how to get
started.

## What's different about Aero?

In the Erlang world, many statically type languages have been popping up, such
as [Alpaca](https://github.com/alpaca-lang/alpaca),
[Gleam](https://github.com/gleam-lang/gleam),
and [Hamler](https://github.com/hamler-lang/hamler). Each has done great things
to get people on board the type safety train.

The goal of Aero is to provide the same foundation seen in the languages listed,
but from a different approach. Aero aims to give the same powerful concurrency
found in Erlang and Elixir, while remaining friendly to those from a background
in the "New C" family of languages, like Swift and Rust, and using uniqueness
types found in languages like Clean while not making purely functional
programming a burden on the developer.
