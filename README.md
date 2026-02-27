# 🪙 Bitcoin Like Blockchain 

A minimal Bitcoin like blockchain implementation written in Rust for learning purposes.

This project is built to understand how real blockchains like Bitcoin work internally including blocks, transactions, mining, wallets, networking, and consensus.

It focuses on **core blockchain features** rather than production security.

---

## 🚀 Core Blockchain Features

### 🔗 Blockchain Structure
- Block & Blockchain data structures  
- Genesis block creation  
- Linked blocks via previous hash  
- Chain validation  
- Fork handling basics  

---

### 💸 Transactions
- Transaction creation & validation  
- Inputs & Outputs structure  
- Transaction hashing  
- Double-spend protection logic  
- Fee support (planned)  
- UTXO model (planned)  

---

### ⛏ Mining (Proof of Work)
- SHA-256 hashing  
- Nonce generation  
- Difficulty target  
- Block reward system  
- Mining reward transaction (coinbase)  
- Difficulty adjustment (planned)  

---

### 🔐 Cryptography
- Public / Private key generation  
- Wallet address creation  
- Digital signatures  
- Signature verification  
- Hashing with SHA-256  
- Merkle tree root (planned)  

---

### 👛 Wallet
- Keypair generation  
- Address generation  
- Balance calculation  
- Transaction signing  
- Import / export keys (planned)  

---

### 🌐 Node Features
- Transaction mempool  
- Block validation  
- Chain synchronization basics  
- Broadcast new transactions  
- Broadcast mined blocks  
- Peer-to-peer networking (planned)  

---

### 📡 Networking (Planned)
- P2P communication  
- Node discovery  
- Gossip protocol  
- Block propagation  
- Transaction propagation  

---

### 🗄 Storage (Planned)
- Persistent blockchain storage  
- UTXO database  
- Wallet storage  
- Block indexing  

---

### ⚖ Consensus
- Proof of Work consensus  
- Longest-chain rule  
- Block verification  
- Difficulty adjustment  

---

### 🛠 Developer Features
- Modular Rust workspace  
- CLI tools for node / wallet / miner  
- Logging & debugging tools  
- Configurable network parameters  
- Test blockchain mode  

---

## 🏗 Project Structure

```

mini-bitcoin-rs/
│
├── lib/        → Core blockchain logic
├── node/       → Node implementation
├── miner/      → Mining engine
├── wallet/     → Wallet & key management
├── Cargo.toml  → Workspace configuration
└── README.md

```

---

## 📚 Learning Objectives

This project helps you understand:

- How Bitcoin blocks are structured  
- How Proof-of-Work secures a network  
- How transactions work using UTXO  
- How wallets create and sign transactions  
- How nodes validate blocks  
- How blockchain consensus works  

---

## 🛠 Installation

### Clone the repository
```
bash
git clone https://github.com/yourusername/mini-bitcoin-rs.git
cd mini-bitcoin-rs
````

### Build workspace

```
bash
cargo build
```

### Run components

```
bash
cargo run -p node
cargo run -p miner
cargo run -p wallet
```

---

## ⚙️ Example Block Structure

```
rust
pub struct Block {
    pub index: u64,
    pub timestamp: u128,
    pub transactions: Vec<Transaction>,
    pub previous_hash: String,
    pub nonce: u64,
    pub hash: String,
}
```

---

## 🎯 Future Improvements

* [ ] Full P2P networking
* [ ] Smart contract support
* [ ] Light node mode
* [ ] REST API & Web dashboard
* [ ] GPU mining simulation
* [ ] Multi-node test network
* [ ] Explorer UI

---

## ⚠️ Disclaimer

This is a simplified educational blockchain implementation.
It is **NOT secure** and should not be used in production.

---

## 👨‍💻 SHAH RUKH RAO

Built with ❤️ in Rust to deeply learn blockchain and distributed systems.

```
