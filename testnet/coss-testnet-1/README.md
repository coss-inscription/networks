# coss-testnet-1
> This is coss testnet chain

> GENESIS PUBLISHED

> PEERS PUBLISHED

1st testnet for coss-inscription/coss application.

## Create fullnode

* Initialize node
```shell
cossd init {{NODE_NAME}}
```
* Replace the contents of your `${HOME}/.coss/config/genesis.json` with that of testnet/coss-testnet-1/genesis.json from the `main` branch of [repository](https://github.com/coss-inscription/networks).
* Copy below node as `persistent_peers` or `seeds` in `${HOME}/.coss/config/config.toml`
```shell
738698413b8afe09aa3724c884251db7fccf37c9@18.181.25.162:26656
```

* Copy below value as minimum-gas-prices in ${HOME}/.coss/config/app.toml
```shell
0ucgas
```

* Start coss by running below command or create a `systemd` service to run coss in background.
```shell
cossd start
```