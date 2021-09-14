## A New Model of Value Exchange

https://medium.com/coinmonks/ipfs-whitepaper-in-four-minutes-b3d5eb0e75c6

Today, HTTP is the de-facto way to transmit files across the internet. It works pretty well to move small files because the process is cheap. But, HTTP fails to take advantage of new file distribution techniques invented in the past decade. 

The upgrades are nearly impossible without breaking backward compatibility and because of the huge investment in the current model of HTTP and the web.
In the coming days, there will be new challenges like:

- Moving datasets in size of petabytes.
- High volume real-time media streams.
- Permanence (to prevent disappearance of important files).

Pretty much every problem boils down to high availability and bigger size. The **InterPlanetary File System (IPFS)** is a peer-to-peer version-controlled filesystem seeking to address these challenges.

**Use cases:**

IPFS provides a generic way to share files and data in a peer to peer fashion optimizing delivery. Some of the use case scenarios where IPFS would be great are:

- Sharing files and huge datasets.
- Serving websites and blogs on IPFS.
- Using as a data source or sink in data processing workflows.
- Using as a Mounted filesystem.
- 
**Conclusion:**

The white-paper discusses a peer-to-peer, version-controlled approach to a filesystem. This filesystem has no single point of failure. Since the data is content-addressed, the nodes in the network don’t need to trust each other. As per this article, IPFS has the potential to replace HTTP and make the web, distributed.

The InterPlanetary File System (IPFS) is a protocol and peer-to-peer network for storing and sharing data in a distributed file system. IPFS uses content-addressing to uniquely identify each file in a global namespace connecting all computing devices.

**Design**

IPFS allows users to host and receive content in a manner similar to BitTorrent. As opposed to a centrally located server, IPFS is built around a decentralized system of user-operators who hold a portion of the overall data, creating a resilient system of file storage and sharing. Any user in the network can serve a file by its content address, and other peers in the network can find and request that content from any node who has it using a distributed hash table (DHT).

In contrast to BitTorrent, IPFS aims to create a single global network. This means that if Alice and Bob publish a block of data with the same hash, the peers downloading the content from Alice will exchange data with the ones downloading it from Bob.

IPFS aims to replace protocols used for static webpage delivery by using gateways which are accessible with HTTP. Users may choose not to install an IPFS client on their device and instead use a public gateway. 

A list of these gateways is maintained on the IPFS GitHub page 

Medusa500 was created by Sadern Alwis, who later founded Mad Tesla's Lab with Omer Nazeer, in May 2021. According to its website and that of Forbes, Mad Tesla's Lab is "an open-source research, development, and deployment laboratory for blockchain technology, using a distribued quantum computing architecture" that "focus on reality defining expansions" and whose goal is to "reimagine life after google with the resonance of human thought, creativy and imagination as the fundamental units of currency"

Mad Tesla's Lab include Medusa500, ....





