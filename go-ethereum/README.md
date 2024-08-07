# What is Go Ethereum?

Go Ethereum is Golang execution layer implementation of the Ethereum protocol.

## Deploy Go Ethereum node on Akash

1. Install [Keplr](https://chrome.google.com/webstore/detail/keplr/dmkamcknogkgcdfhhbddcghachkejeap) wallet as a browser extension
2. Fund your wallet with at least 5 AKT. How to get AKT? Read at https://akash.network/token
3. Open [Cloudmos](https://deploy.cloudmos.io/) or [Akash Console](https://console.akash.network/) and connect your Keplr wallet
5. Create a certificate
3. Create deployment
4. Choose `Empty` for the template and copy-and-paste the `deploy.yaml` file from this repository

Click [here](https://docs.akash.network/guides/deploy) to learn more about deploying.

## Get Access to Ethereum RPC

List of example JSON-RPC calls can be found [here](https://ethereum.org/en/developers/docs/apis/json-rpc/)

For example:
```
curl -H "Content-Type: application/json" -X POST --data '{"jsonrpc":"2.0","method":"web3_clientVersion","params":[],"id":67}' http://localhost:8545
```
Use URI from Cloudmos or Akash Console after deployment instead of http://localhost:8545

## Documentation

[Go Ethereum on Github](https://github.com/ethereum/go-ethereum)
[Getting started with Geth](https://geth.ethereum.org/docs/getting-started)
[JSON-RPC API](https://ethereum.org/en/developers/docs/apis/json-rpc/)
[Docker Hub](https://hub.docker.com/r/ethereum/client-go/tags)
