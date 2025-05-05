# Blockchain Explorer - Add New Chain Guide  

## How to Add a New Chain  

### 1. Prepare Chain Information  
Create a JSON file with your chain's specifications:  

```json
{
    "chain_name": "atomone",
    "favorite": "true",
    "chain_id": "atomone-1",
    "validator_address": "atonevaloper15e709ulu0sxgpwzu3vftkxd00eexapmj76e7kh",
    "registry_name": "atomone",
    "network_type": "mainnet",
    "codebase": {
        "github_org": "atomone-hub"
    },
    "api": [
        {
            "address": "https://atomone-mainnet-api.itrocket.net"
        }
    ],
    "rpc": [
        {
            "address": "https://atomone-mainnet-rpc.itrocket.net"
        }
    ],
    "sdk_version": "0.45.1",
    "coin_type": "118",
    "min_tx_fee": "800",
    "theme_color": "#161723",
    "addr_prefix": "atone",
    "logo": "/logos/atomone.png",
    "assets": [
        {
            "base": "uatone",
            "symbol": "atone",
            "exponent": "6",
            "coingecko_id": "atomone",
            "logo": "/logos/atomone.png"
        }
    ]
}

```
2. File Placement
Add JSON file to /chains/yourchain.json

Add logo (256x256 PNG) to /public/logos/yourchain.png

3. Naming Requirements
JSON filename must match icon field (e.g., yourchain.json)

Logo filename must exactly match the icon value

4. Submit Changes
Create a pull request with:

Your chain JSON file

Properly sized logo

Accurate chain information

[Sample PR Title] "feat: Add support for YourChain"

