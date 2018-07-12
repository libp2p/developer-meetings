# Scaling DHT to millions of nodes

## Current Shortcomming

- No backoff mechanism - The DHT gets abused by other protocols constantly
- Membership problem - Everyone gets to be a DHT, causes a lot of churn
- No protection to flash crowds (aka sybil attacks)

## Candidate solutions

- **Backoff mechanism** - 
- **Coordination Protocol** - 
- **Sane defaults for connection Management** - 
- **Crypto Puzzles for when flash crowds happen** - 
- **Network Layout Recipes for specific use cases (e.g. "Dias-Peer-Set" for PeerPad, X for Social Networks, Y for Live Streaming)** - 
- **Proxy reencryption for Gossip (blind bridge)** - Share nodes and network state through Gossip protocol 
- **Describe the network state in a signed IPLD graph** - (needs an accumulator)
- **membership mechanism** - Nodes should have to prove their worth (or their ability) to be parts of more sensitive protocols (i.e. time alive challenge)


## Reference for Scaling DHTs

- Vivalvi with geobandwidth location 
- Coral with DHT clusting
- AnonRep and other Reputation Papers



## Other, still to be organized

- Options for the users to control the number of connections

- Nodes should not need more than 100 to 300 conns. Some nodes won’t be able to have more than 30 (i.e. browsers)
- DHT should have a backoff mechanism
- There should be some kind of coordination service that tells the health of the DHT so that nodes can provide better heuristics to what is happening.
- Reputation is big part of this


