# Blockchain Snapshots Service 

A snapshot is a file that stores the present condition of a blockchain at a specific moment in time. This snapshot encompasses the entire blockchain ledger, documenting every existing address and its associated details, such as transactions, fees, balances, metadata, and more, and it's kept in a folder on your hard drive.

Whenever a node decides to join the network, it must download the entire blockchain history, starting sync from the first block (genesis block) to the most recent block produced. The size of this blockchain can vary significantly, ranging from 10-50 GB to as much as a few TBs. In contrast, snapshots provide an efficient alternative, allowing nodes to synchronize with the network by downloading only the latest state data.

We provide Blockchain Snapshots Service for selected chains as a part of our infrastructure offering bundled with [Block Explorer as a service.](https://b2b.dex.guru/explorer) 


## Canto Network Blockchain Snapshot

### Snapshot Details

This snapshot is an archive of the Canto Network blockchain data, capturing the state up to 7926390 block. It is designed for node operators or individuals looking to quickly sync with the network.

- **Snapshot Size:** Approximately 2200GB.
- **Required Free Space:** At least 2500GB on the node to accommodate unpacking and future growth.
- **Snapshot URL:** [https://storage.googleapis.com/evm_snapshots/canto/canto_7700-1_2024-01-23.tar](https://storage.googleapis.com/evm_snapshots/canto/canto_7700-1_2024-01-23.tar)

Please note, the download speed may vary based on your internet connection and server bandwidth.

### Downloading and Using the Snapshot

To download and unpack the snapshot without storing the entire archive on your node, use the following command:

```bash
wget -O- https://storage.googleapis.com/evm_snapshots/canto/canto_7700-1_2024-01-23.tar | tar -xv
```

Additional Information
- This snapshot is provided as-is for the community's convenience, without guarantees regarding completeness beyond the specified block.
- Ensure your node meets the above requirements for storage space and network capacity before proceeding.
---------------------------------
## Manta Network Blockchain Snapshot

### Snapshot Details

This snapshot is an archive of the Manta Network blockchain's geth directory, capturing the state up to block ~1213370. It is intended for use by node operators or individuals looking to quickly sync with the network without processing all transactions from genesis.

- **Snapshot Size:** Approximately 100GB.
- **Required Free Space:** At least 120GB on the node to accommodate unpacking and future growth.
- **Snapshot URL:** [https://storage.googleapis.com/evm_snapshots/manta/geth_20240127120858.tar](https://storage.googleapis.com/evm_snapshots/manta/geth_20240127120858.tar)

Please note, this is a public link, and download speed may be limited based on your internet connection and server bandwidth.

### Downloading and Using the Snapshot

To efficiently download and use the snapshot without storing the entire archive on your node, you can use the following `wget` command piped into `tar` to extract the files directly:

```bash
wget -O- https://storage.googleapis.com/evm_snapshots/manta/geth_20240127120858.tar | tar -xv
```

This command downloads the snapshot and extracts it on-the-fly, reducing the need for additional storage space during the setup process.

## Additional Information
- This snapshot is provided "as is" for convenience, with no guarantees regarding up-to-dateness or completeness beyond block 844,730.
- Ensure your node meets the specified requirements before attempting to use this snapshot, including available storage space and network connectivity.

