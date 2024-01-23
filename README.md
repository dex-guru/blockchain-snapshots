# Manta Network Blockchain Snapshot

## About Manta Network

Manta Network is a privacy-preserving decentralized finance (DeFi) platform built on Substrate, designed to offer private transactions and swaps for blockchain assets. Leveraging zk-SNARKs, Manta Network aims to provide high-throughput and privacy-focused blockchain solutions, enabling users to transact and exchange cryptocurrencies with privacy and security at its core.

## Key Features of Manta Network

- **Privacy-Preserving Transactions:** Utilizes zk-SNARKs to ensure transactions remain confidential while still being verifiable on the blockchain.
- **High Throughput:** Designed to support a high number of transactions per second (TPS), catering to the scalability needs of DeFi and other applications.
- **Interoperability:** Built on Substrate, Manta Network is designed for cross-chain compatibility within the Polkadot ecosystem, enhancing its reach and utility.
- **User-Friendly:** Offers a seamless experience for users looking to conduct private transactions or swaps without compromising on speed or security.

## Snapshot Details

This snapshot is an archive of the Manta Network blockchain's geth directory, capturing the state up to block 844,730. It is intended for use by node operators or individuals looking to quickly sync with the network without processing all transactions from genesis.

- **Snapshot Size:** Approximately 50GB
- **Required Free Space:** At least 70GB on the node to accommodate unpacking and future growth.
- **Snapshot URL:** [https://storage.googleapis.com/evm_snapshots/manta/geth.tar](https://storage.googleapis.com/evm_snapshots/manta/geth.tar)

Please note, this is a public link, and download speed may be limited based on your internet connection and server bandwidth.

## Downloading and Using the Snapshot

To efficiently download and use the snapshot without storing the entire archive on your node, you can use the following `wget` command piped into `tar` to extract the files directly:

```bash
wget -O- https://storage.googleapis.com/evm_snapshots/manta/geth.tar | tar -xv
```

This command downloads the snapshot and extracts it on-the-fly, reducing the need for additional storage space during the setup process.

## Additional Information
- This snapshot is provided "as is" for convenience, with no guarantees regarding up-to-dateness or completeness beyond block 844,730.
- Ensure your node meets the specified requirements before attempting to use this snapshot, including available storage space and network connectivity.

For more information about Manta Network and its features, please visit the official [Manta Network website](https://manta.network/).
