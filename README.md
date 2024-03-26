# Blockchain Snapshots Service 

A snapshot is a file that stores the present condition of a blockchain at a specific moment in time. This snapshot encompasses the entire blockchain ledger, documenting every existing address and its associated details, such as transactions, fees, balances, metadata, and more, and it's kept in a folder on your hard drive.

Whenever a node decides to join the network, it must download the entire blockchain history, starting sync from the first block (genesis block) to the most recent block produced. The size of this blockchain can vary significantly, ranging from 10-50 GB to as much as a few TBs. In contrast, snapshots provide an efficient alternative, allowing nodes to synchronize with the network by downloading only the latest state data.

We provide Blockchain Snapshots Service for selected chains as a part of our infrastructure offering bundled with [Block Explorer as a service.](https://b2b.dex.guru/explorer) 


## CrossFi Mainnet Blockchain Archive Node Snapshot

### Snapshot Details
This section introduces snapshots for the CrossFi blockchain, designed to help node operators and individuals synchronize with the CrossFi network quickly. For the latest snapshot details, including the block height and size, please visit the provided link.

### Snapshot URL: [https://storage.googleapis.com/evm_snapshots/crossfi/index.html](https://storage.googleapis.com/evm_snapshots/crossfi/index.html)

The link directs to an index page where the most recent snapshot of the CrossFi blockchain is available. This snapshot is crucial for those looking to rapidly integrate and sync with the CrossFi network, bypassing the need to process every transaction from the genesis block.
The snapshot must be unpacked to "home" blockchain directory (which can be indicated by using **--home** argument) with name **data**

### example:
├── bin
│   ├── crossfid
└── testnet
    ├── config
    ├── data  <----


### Downloading and Using the Snapshot
Details on how to download and apply the snapshot can be found on the index page. Typically, the process involves using a command similar to those provided for other blockchains, allowing for efficient downloading and unpacking of the snapshot data.

### Additional Information
The CrossFi snapshot is provided "as is" for the community's convenience. Please verify the snapshot's completeness and up-to-dateness as per your requirements.
Ensure your node meets the necessary requirements for storage space and network connectivity before attempting to utilize the snapshot.
This addition ensures that users interested in the CrossFi blockchain can quickly access and utilize the latest snapshot for their nodes, facilitating easier and faster synchronization with the network.

## Canto Mainnet blockchain archive node snapshot

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
## Manta Mainnet blockchain archive node snapshot

### Snapshot Details

This snapshot is an archive of the Manta Network blockchain's geth directory, capturing the state up to block ~137800. It is intended for use by node operators or individuals looking to quickly sync with the network without processing all transactions from genesis.

- **Snapshot Size:** Approximately 131GB.
- **Required Free Space:** At least 150GB on the node to accommodate unpacking and future growth.
- **Snapshot URL:** [https://storage.googleapis.com/evm_snapshots/manta/eth_20240215124815.tar](https://storage.googleapis.com/evm_snapshots/manta/eth_20240215124815.tar)

Please note, this is a public link, and download speed may be limited based on your internet connection and server bandwidth.

### Downloading and Using the Snapshot

To efficiently download and use the snapshot without storing the entire archive on your node, you can use the following `wget` command piped into `tar` to extract the files directly:

```bash
wget -O- https://storage.googleapis.com/evm_snapshots/manta/eth_20240215124815.tar | tar -xv
```

This command downloads the snapshot and extracts it on-the-fly, reducing the need for additional storage space during the setup process.

## Additional Information
- This snapshot is provided "as is" for convenience, with no guarantees regarding up-to-dateness or completeness beyond block 844,730.
- Ensure your node meets the specified requirements before attempting to use this snapshot, including available storage space and network connectivity.
---------------------------------
# Optimism Mainnet blockchain archive node snapshot

## Snapshot Details

This snapshot is an archive of the Optimism blockchain's geth directory, capturing the state up to ~115381265 block. It is intended for use by node operators or individuals looking to quickly sync with the Optimism network without processing all transactions from the genesis block.

- Snapshot Size: Approximately 3700GB.
- Required Free Space: At least 4000GB on the node to accommodate unpacking and future growth.
- Snapshot URL: [https://storage.googleapis.com/evm_snapshots/optimism/geth_20240127132251.tar](https://storage.googleapis.com/evm_snapshots/optimism/geth_20240127132251.tar)

Please note, this is a public link, and download speed may be limited based on your internet connection and server bandwidth.

## Downloading and Using the Snapshot

To efficiently download and use the snapshot without storing the entire archive on your node, you can use the following command piped into tar to extract the files directly:

```bash
wget -O- https://storage.googleapis.com/evm_snapshots/optimism/geth_20240127132251.tar | tar -xv
```

This command downloads the snapshot and extracts it on-the-fly, reducing the need for additional storage space during the setup process.

## Additional Information
- This snapshot is provided "as is" for convenience, with no guarantees regarding up-to-dateness or completeness beyond block 115381265.
- Ensure your node meets the specified requirements before attempting to use this snapshot, including available storage space and network connectivity.
