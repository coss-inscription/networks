# coss-1
> This is coss mainnet chain

> GENESIS PUBLISHED

> PEERS PUBLISHED

mainnet for coss-inscription/coss application.

## Create fullnode

* Initialize node
```shell
cossd init {{NODE_NAME}}
```
* Replace the contents of your `${HOME}/.coss/config/genesis.json` with that of main/v1/genesis.json from the `main` branch of [repository](https://github.com/coss-inscription/networks).
* Copy below node as `persistent_peers` or `seeds` in `${HOME}/.coss/config/config.toml`
```shell
9f0a41abda8e08edc64d27ecc4edeef1941d70c0@172.31.37.139:26656,2f2815602ac270224c913dbddc6b7f8d0a6fd052@172.31.47.245:22656
```

* Copy below node as `timeout_propose` in `${HOME}/.coss/config/config.toml`
```shell
10s
```

* Copy below node as `timeout_commit` in `${HOME}/.coss/config/config.toml`
```shell
10s
```

* Copy below value as `minimum-gas-prices` in ${HOME}/.coss/config/app.toml
```shell
"0.025ucgas,0.025ucoss"
```

* Start coss by running below command or create a `systemd` service to run coss in background.
```shell
cossd start
```
