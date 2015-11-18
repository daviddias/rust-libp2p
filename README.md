[libp2p](https://github.com/ipfs/specs/tree/master/protocol/network) Implementation in Rust
===========================================================================================

> libp2p implementation in Rust

# Description

libp2p is a networking stack and library modularized out of The IPFS Project, and bundled separately for other tools to use.

libp2p is the product of a long, and arduous quest of understanding -- a deep dive into the internet's network stack, and plentiful peer-to-peer protocols from the past. Building large scale peer-to-peer systems has been complex and difficult in the last 15 years, and libp2p is a way to fix that. It is a "network stack" -- a protocol suite -- that cleanly separates concerns, and enables sophisticated applications to only use the protocols they absolutely need, without giving up interoperability and upgradeability. libp2p grew out of IPFS, but it is built so that lots of people can use it, for lots of different projects.

We will be writing a set of docs, posts, tutorials, and talks to explain what p2p is, why it is tremendously useful, and how it can help your existing and new projects.

# Usage

`rust-libp2p` repo will be a place holder for the list of Rust modules that compose Rust libp2p.

# Modules

- [libp2p] (entry point)
- **Swarm**
  - [libp2p-swarm]()
  - [libp2p-identify]()
  - [libp2p-ping]()
  - Transports
    - [abstract-transport](https://github.com/diasdavid/abstract-transport)
    - [abstract-connection](https://github.com/diasdavid/abstract-connection)
    - [libp2p-tcp]()
    - [libp2p-udp]()
    - [libp2p-udt]()
    - [libp2p-utp]()
    - [libp2p-webrtc]()
    - [libp2p-cjdns]()
  - Stream Muxing
    - [abstract-stream-muxer](https://github.com/diasdavid/abstract-stream-muxer)
    - [libp2p-spdy]()
    - [libp2p-multiplex]()
  - Crypto Channel
    - [libp2p-tls]()
    - [libp2p-secio]()
- **Peer Routing**
  - [libp2p-kad-routing]()
  - [libp2p-mDNS-routing]()
- **Discovery**
  - [libp2p-mdns-discovery]()
  - [libp2p-random-walk]()
  - [libp2p-railing]()
- **Distributed Record Store**
  - [libp2p-record]()
  - [abstract-record-store](https://github.com/diasdavid/abstract-record-store)
  - [libp2p-distributed-record-store]()
  - [libp2p-kad-record-store]()
- **Generic**
  - [PeerInfo]()
  - [PeerId]()
  - [multihash]()
  - [multiaddr]()
  - [multistream]()
  - [multicodec]()
  - [ipld]()
  - [repo]()
- [**Specs**](https://github.com/ipfs/specs/tree/master/protocol/network)
