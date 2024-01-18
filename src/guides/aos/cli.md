# CLI

There are some command-line arguments you pass to our aos to do the following:

- [name] - create a new process or loads an existing process for your wallet
- --load [file] - load a file, you can add one or many of this command
- --cron [interval] - only used when creating a process
- --wallet [walletfile] - use a specific wallet

## Managing multiple processes with aos

```sh
aos
```

Starts or connects to a process with the name `default`

```sh
aos chatroom
```

Starts or connects to a process with the name of `chatroom`

```sh
aos treasureRoom
```

Starts or connects to a process with the name of `treasureRoom`

## Load flag

```sh
aos treasureRoom --load greeting.lua --load treasure.lua --load puzzle.lua
```

With the load flag I can load many source files to my process

## CRON Flag

If you want to setup your process to react on a schedule we need to tell ao, we do that when we spawn the process.

```sh
aos chatroom --cron 2-minutes
```