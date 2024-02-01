## Floodsub poster

### How does floodsub work?
- Each peer subscribing to topic X sends every X-type message to every other peer
it knows who is subscribing (except the one it received the message from)

- Example:  5 peers where each one is connected to every other peer.  Then each
peer would receive 4 copies => 20 total messages

- What if none of my peers subscribe to the topic that I am subscribed to?  Do I
get any messages? No.  Solution is rendezvous protocol.

- What are the guarantees provided by FloodSub?
	- How many malicious nodes will make floodsub unusable

### Problems & Challenges

	1. Scalability - b/c this is an intentionally naive PubSub implementation
	2. Rendezvous - needs to be developed
	3. Authenticated messages to prevent spam
	4. Fault tolerance - failure of a peer to send messages to you due to crash is indistinguishable from case where no messages are being sent on that topic

### How to contribute / where is the code?

- Repo:  libp2p/go-floodsub

- Best type of contributor: 

	- Wants to work on gossipsub (next generation), which is still in the research stage
	- High bandwidth requirement from team in terms of settling on proposed path
ahead: eagerness to interact with Kubuxu or Stebalien in working through next
solutions ahead of PR
	- Current status:  vyzo has simulation in LISP; no production implementation yet


### Where does floodsub fits in the pubsub landscape?

- Simple and easy to implement pubsub protocol

- There are other implementation and research effort going on. gossipsub is
designed to be a general purpose, robust, scalable easy to implement pubsub
protocol. It is backwards compatible with gossipsub.

- Gossipsub goal is to be the general purpose pubsub protocol, but other protocols
will be implemented and used depending on the specific purpose (e.g. video
stream would require a specialized protocol).

- Floodsub and gossipsub are meant to be the UDP of pubsub, offering no order
guarantees or reliability. Those properties can be added on top of it (example:
pulsarcast https://github.com/ipfs/notes/issues/266) 

QA about gossipsub and pubsub efforts https://github.com/libp2p/go-floodsub/issues/77

