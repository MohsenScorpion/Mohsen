# Mohsen

curl https://eth-mainnet.g.alchemy.com/v2/nsmQNhA9OA2tYQkFNu2_ZooFb8hpIEdE -X POST -H "Content-Type: application/json" -d '{"jsonrpc":"2.0","method":"eth_getBlockByNumber","params":["latest", false],"id":0}'

npm install alchemy-sdk

import { Network, Alchemy } from 'alchemy-sdk';

const settings = {
    apiKey: "nsmQNhA9OA2tYQkFNu2_ZooFb8hpIEdE",
    network: Network.ETH_MAINNET,
};

const alchemy = new Alchemy(settings);

// get the latest block
const latestBlock = alchemy.core.getBlock("latest").then(console.log);


node script-name.js


pip install web3


# Setup
from web3 import Web3

alchemy_url = "https://eth-mainnet.g.alchemy.com/v2/nsmQNhA9OA2tYQkFNu2_ZooFb8hpIEdE"
w3 = Web3(Web3.HTTPProvider(alchemy_url))

# Print if web3 is successfully connected
print(w3.isConnected())

# Get the latest block number
latest_block = w3.eth.get_block("latest")
print(latest_block)

python <your_filename>.py
