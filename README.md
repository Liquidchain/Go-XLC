## Official Golang implementation of the Liquidchain Network.

Liquidchain is a layer-1 blockchain powered by Proof of Authority (PoA) consensus mechanism compatible to Ethereum Virtual Machine (EVM). It is specially designed for liquidity providers and DeFi users. Unlike Ethereum, Liquidchain is secured by a group of trusted validators who utilizes PoA algorithm, which is more efficient than Ethereum’s Proof of Work (PoW). Validators generate blocks and earn from the txn fees. Liquidchain is scalable, extremely cheaper and faster L1 blockchain.

Website: https://liquidchain.net | 
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

Keep geth running

```tmux new -s node```

Testnet

```./geth init xlc_testnet.json --datadir ./data```

```./geth --datadir ./data --syncmode 'full' --port 5051 --networkid 5051 --nodiscover```





