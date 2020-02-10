# 6miner

6miner is a highly optimized cryptocurrency miner that runs on modern AMD / NVIDIA GPUs and CPUs. 
* 6miner currently supports [handshake](https://handshake.org/)(blake2b + sha3) algorithm with 3% of devfee.

## Quick start
* [Download](https://github.com/6block/6miner/releases/latest) and extract 6miner into a folder.
* Depending on the coins that you want to mine, find the corresponding script in the folder.(e.g `mine_hns.sh`, `mine_hns.b at`).
* Change the address and vendor information in the script.
* Run the script and Enjoy mining.

## Reference performances
| algorithm | card | hashrate | 
| --- | --- | --- |
| handshake(blake2b + sha3) | 2080 Ti | 460MH/s |
| handshake(blake2b + sha3) | 1080 Ti | 350MH/s |
| handshake(blake2b + sha3) | 2060 | 185MH/s |
| handshake(blake2b + sha3) | RX 580 | 64MH/s |
| handshake(blake2b + sha3) | Tesla T4 | 220MH/s |
| handshake(blake2b + sha3) | P100 | 100MH/s |


## Command line options
```
  -a, --algo=ALGO           specify the algorithm to use
  -o, --url=URL             URL of mining server
  -u, --user=USERNAME       username for mining server
  -p, --pass=PASSWORD       password for mining server
  -m, --mode=MODE           options: CPU\CUDA\OpenCL. (default: CPU)
      --devices=0,1,2       list of GPU devices to use. (default: all)
      --temperature-limit=N limit maximun temperature of GPU. (default: 90)
      --opcl-vendor=VENDOR  vendor name for OpenCL mode. (default: AMD, options: AMD NVIDIA Intel).
      --opcl-no-cuda-fix    disable lower cpu usage for OpenCL mode using Nvidia cards.
      --threads=N           count of CPU threads for CPU mode.
  -h, --help                display this help and exit
  -V, --version             output version information and exit
```
