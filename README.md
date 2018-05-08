# AmoveoMinerMan
Miner for Amoveo blockchain
This miner is optimized for CUDA code, which is designed for Nvidia devices. So AMD cards can not run this miner at present.

## Usage:
- First you'll need to run "AmoveoMinerMan.exe 2" to find and optimize your system. (1 time step)
- You can run "AmoveoMinerMan.exe 1" to benchmark current config or "AmoveoMinerMan.exe 0" to start mining
There is a lag or system hang while optimizing, so be patient and wait. Edit *your wallet address* inside config.txt

## Known performance:
- GTX 1080Ti: 4.7 GH/s
- GTX 1080: ??
- GTX 1070Ti: ??
- GTX 1060: ??
- GTX 1050: ??
- GTX 970: 1.2 GH/s
## Known issue:
- GPUs getting hotter than normal version ~4-5 Celsius
- Lag and hang on Windows since we use total mem/cores in display GPU.

## Linux

### Linux Install dependencies

```
sudo apt-get install libcpprest-dev libncurses5-dev libssl-dev unixodbc-dev g++ git
```

##TODO
So far, we are using the same algorithm with Mandelhoff. Me and my guys are developing different approach to improve the performance soon.
