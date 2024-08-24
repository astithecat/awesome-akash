# Celo
Set up your CELO Mainnet or Alfajores Testnet RPC node

## Deploy Celo on Akash
Deploy on Akash Console using the required SDL
- Deploy Celo Mainnet with [deploy_mainnet.yaml](https://github.com/astithecat/awesome-akash/blob/celo/celo/deploy_mainnet.yaml)
- Deploy Celo Alfajores with [deploy_alfajores.yaml](https://github.com/astithecat/awesome-akash/blob/celo/celo/deploy_alfajores.yaml)

Don't forget to fill the env <CELO_ACCOUNT_ADDRESS> with your public wallet address int. You can create a wallet [here](https://celowallet.app/setup)

## Check Synced
To test your Celo RPC node, you can send an RPC request using cURL
```
curl https://localhost:8545 \
--request POST \
--header "Content-Type: application/json" \
--data '{ "jsonrpc":"2.0", "method":"eth_syncing","params":[],"id":1}'
```
