<h1 align=center>0G LABS: Storage Node</h1>

![0_AxKIus_I-soNSp03](https://github.com/user-attachments/assets/eb3cd7ae-d588-4d3a-8096-60be1838a1c5)

# Storage Node
## Hardware Requirement
|Field|Value|
|:----|:----|
|Memory|16 GB|
|CPU|4 cores|
|Disk| 500 GB / 1 TB NVME SSD|
|Bandwidth|500 MBps for Download / Upload|

## Install via CLI
```bash
git clone https://github.com/0glabs/0g-storage-client.git
cd 0g-storage-client
go build
./0g-storage-client upload --url <blockchain_rpc_endpoint> --contract <log_contract_address> --key <private_key> --node <storage_node_rpc_endpoint> --file <file_path>
./0g-storage-client download --node <storage_node_rpc_endpoint> --root <file_root_hash> --file <output_file_path>
./0g-storage-client download --node <storage_node_rpc_endpoint> --root <file_root_hash> --file <output_file_path> --proof
```
