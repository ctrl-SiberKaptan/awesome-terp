Resources
This section includes official, developer, community, and social resources.

Official Resources
TerpNet Website — https://terp.network
TerpNet Explorer — https://explorer.terp.network
TerpNet MarketPlace — https://marketplace.terp.network
TerpNet Devnet — https://devnet.terp.network
TerpNet Blog — https://blog.terp.network
TerpNet Documentation — https://docs.terp.network
TerpNet RPC — https://rpc.terp.network
TerpNet REST or LCD — https://rest.terp.network
Developer repositories
Terp-Core Repository — https://github.com/terpnetwork/node
Devnet Repository — https://github.com/terpnetwork/webApp
Official Endpoints
We provide following endpoints to help developers for integration

Protocol	Endpoints
RPC	https://rpc.terp.network
REST	https://rest.terp.network
GRPC	grpc://grpc.terp.network
WSS	wss://rpc.terp.network:443/websocket
State-Sync
To use statesync, change the following under config.toml

[statesync]
enable = true
rpc_servers = "https://rpc.terp.network:443,https://rpc.terp.network:443"
trust_height = 0
trust_hash = ""
trust_period = "112h0m0s"
and use a trusted height from the rpc, recent height will work as well

curl -s https://rpc.terp.network/status | jq '.result .sync_info | {trust_height: .latest_block_height, trust_hash: .latest_block_hash} | values'
Validator Contributions
This section includes validator contributions:

Wallets

Explorer

Relayers

RPCs

Bots & Toolings
