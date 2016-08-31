# GossipDB
A distributed document store where transaction acceptance is governed by each node's own rules. If nodes follow the same rules, eventual consistency for these records is achieved.

## Concept
Traditional blockchain networks like bitcoin can be viewed as an eventually consistent distributed document store with a common set of rules for transaction acceptance. These blockchains are very specific in the data they store and in the acceptance rules. While other projects like Ethereum are open for smart contracts, they still have the drawback of being public, mining required as part of the acceptance, ethereum that is needed as gas,...

GossipDB only contains the peer to peer networking and the actual storing of the transactions. No assumptions are made on the content of the data or on the rules, the concept of a block is not even known.
GossipDB is suitable for custom blockchain alike applications storing arbitrary data with custom acceptance rules. These custom acceptance rules might be traditional blocks with mining, enterprise policies with voting distributed to the board or just some nodes having the right to create entries and other nodes to update.

## Examples
Some examples of applications that can be created using GossipDB:
* High availability website with offsite replica's
* A normal virtual currency with blocks and miners
* A distributed identity system with partially shared identities
* A distributed encrypted notary
* ...
