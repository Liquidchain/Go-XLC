## Official Golang implementation of the Liquidchain Network.

Website: https://liquidchain.net
Docs: https://docs.liquidchain.net


## Building the source

Liquidchain Network is forked from Go Ethereum.

Building `geth` requires both a Go (version 1.14 or later) and a C compiler. You can install
them using your favourite package manager. Once the dependencies are installed, run

```shell
make geth
```

or, to build the full suite of utilities:

```shell
make all
```


## Running a Node

`Keep geth running`

```tmux new -s node```

`Testnet`

```./geth init xlc_testnet.json --datadir ./data```

```./geth --datadir ./data --syncmode 'full' --port 5051 --networkid 5051 --nodiscover```





