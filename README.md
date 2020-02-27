# 6miner

6miner is a highly optimized cryptocurrency miner that runs on modern AMD / NVIDIA GPUs and CPUs. 

* 6miner currently supports [handshake](https://handshake.org/)(blake2b + sha3) algorithm with 3% of devfee.

## Quick start

* [Download](https://github.com/6block/6miner/releases/latest) and extract 6miner into a folder.
* Depending on the coins that you want to mine, find the corresponding script in the folder.(e.g `mine_hns.sh`, `mine_hns.b at`).
* Change the address and vendor information in the script.
* Run the script and Enjoy mining.

## Reference performances

| Algorithm                 | Brand  | card       | hashrate |
| ------------------------- | ------ | ---------- | -------- |
| handshake(blake2b + sha3) | AMD    | RX 470     | 145MH/s  |
| handshake(blake2b + sha3) | AMD    | RX 570     | 150MH/s  |
| handshake(blake2b + sha3) | AMD    | RX 580     | 165MH/s  |
| handshake(blake2b + sha3) | AMD    | Vega56     | 282MH/s  |
| handshake(blake2b + sha3) | AMD    | 5700       | 200MH/s  |
| handshake(blake2b + sha3) | AMD    | 5700xt     | 254MH/s  |
| handshake(blake2b + sha3) | AMD    | Radeon Vii | 360MH/s  |
| handshake(blake2b + sha3) | Nvidia | 2060       | 200MH/s  |
| handshake(blake2b + sha3) | Nvidia | P100       | 260MH/s  |
| handshake(blake2b + sha3) | Nvidia | 1080 Ti    | 350MH/s  |
| handshake(blake2b + sha3) | Nvidia | 1660ti     | 257MH/s  |
| handshake(blake2b + sha3) | Nvidia | 1660       | 194Mh/S  |
| handshake(blake2b + sha3) | Nvidia | 1070ti     | 270MH/s  |
| handshake(blake2b + sha3) | Nvidia | 2070Super  | 350MH/s  |
| handshake(blake2b + sha3) | Nvidia | 2080 Ti    | 500MH/s  |
| handshake(blake2b + sha3) | Nvidia | 2080       | 402Mh/s  |
| handshake(blake2b + sha3) | Nvidia | 2080Super  | 440Mh/s  |

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

Here's a detailed how-to on getting started and mining on 6block.com with 6miner!

https://documents.6block.com/how-to-use-6miner
