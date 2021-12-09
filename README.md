## Official Golang implementation of the Liquidchain Network.

Liquidchain is a layer-1 blockchain powered by Proof of Authority (PoA) consensus mechanism compatible to Ethereum Virtual Machine (EVM). It is specially designed for liquidity providers and DeFi users. Unlike Ethereum, Liquidchain is secured by a group of trusted validators who utilizes PoA algorithm, which is more efficient than Ethereum’s Proof of Work (PoW). Validators generate blocks and earn from the txn fees. Liquidchain is scalable, extremely cheaper and faster L1 blockchain.

Liquidchain is the first to introduce Network Integrated AMM Protocol which rewards native cryptocurrency for providing on-chain liquidity. We have implemented this innovative approach to reward our liquidity providers. Usually in all the existing AMM Protocols, there is a governance token which LPs get for providing liquidity. Often the token has no actual utility or use case rather than being a farmed token. But Liquidchain rewards the liquidity providers with the native XLC which can be thought as this - “Uniswap is rewarding ETH or Pancakeswap is rewarding BNB for providing liquidity.” XLC has similar utilities as ETH, BNB, it can be used to pay the network fees, interact with EVM and so on.

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



Bootnodes

Mainnet: ```enode://c227a759af896651a14a99c037a386b468e5a97843d0f1f27ef03c8c19ba2f3a8d8283abbe19c66b019f49bca594393140b157c9b67ee4dde0ec6f3fe5902f4b@207.148.17.132:5050```





