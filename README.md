# Trader Joe Subgraphs

Subgraph for Trader Joe on AVAX chain. 

Forked from `sushiswap-subgraph`. 

### Deploy

```` 
# authenticate api key
$ graph auth https://api.thegraph.com/deploy/ <API_KEY>

# build constants
$ cd packages/constants
$ yarn prepare:avax

# build subgraph
$ cd subgraphs/exchange
$ yarn prepare:avax
$ yarn codegen:avax
$ yarn build:avax

# deploy subgraph
$ yarn deploy:avax
````


### Query

GraphQL endpoints can be found at TheGraph legacy explorer: 
https://thegraph.com/legacy-explorer/subgraph/traderjoe-xyz/exchange