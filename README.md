# AmoveoMinerMan
Miner for Amoveo blockchain
This miner is optimized for CUDA code, which is designed for Nvidia devices. So AMD cards can not run this miner at present.

## Usage:
Just run the executable file, everything will be done automatically.
#### While mining:
- Press [i] then [enter] to see share infomation.
- Press [q] then [enter] to exit.

  
#### If you are Linux miner, just don't care about below lines.
### For Windows miner
- In order to run this miner please do as the following document to turn off WDDM TDR: https://docs.nvidia.com/gameworks/content/developertools/desktop/timeout_detection_recovery.htm

Your NVIDIA Nsight should be like this:
![alt text](https://docs.nvidia.com/gameworks/content/developertools/desktop/images/nsight_monitor_general.002.png)

- By default, FORCE_FULL_INTENSITY_DISPLAY_ACTIVE is auto-disabled for windows user, this flag prevents lag and freezes while mining. Actually, this is a trade-off, hash rate of the display GPU should be decreased by 20%.
- To turn on this flag FORCE_FULL_INTENSITY_DISPLAY_ACTIVE please add FORCE_FULL_INTENSITY_DISPLAY_ACTIVE at the end of the config file.

## If you have troubles while running the miner, please run Debug version and post the issue on this repo. We are pleased to help you.

Remember to Edit *your wallet address* inside config.txt

## Config example (config.txt & deviceconfig.txt)
### config.txt
```
your_address <required>
pool_URL <required>
flag <optional>
```
### deviceconfig.txt (we recommend you run AmoveoMinerMan 2 instead of editing this file manually)
```
number of device
device id 0 block size number of blocks
device id 1 block size number of blocks
device id 2 block size number of blocks
```
  
## Known performance:
- GTX 1080Ti: 4.7 GH/s (5.2 GH/s for OC cards)
- GTX 1080: ??
- GTX 1070Ti: ??
- GTX 1060: ??
- GTX 1050: ??
- GTX 970: 1.7 GH/s
## Known issue:
- GPUs getting hotter than normal version ~4-5 Celsius
- Lag and hang on Windows since we use total mem/cores in display GPU.

## Linux

### Linux Install dependencies

```
sudo apt-get update
sudo apt-get install libcpprest2.8 libcpprest-dev libncurses5-dev libssl-dev unixodbc-dev g++ git
```

## TODO
- So far, we see many new techniques to improve this miners. But we need to collect more feedback to finalize basic things.
- Porting the code to OpenCL: We are currently waiting for the money that comes from VEO donation in order to buy AMD hardwares. If you really want us to create AMD_VeoMiner, please donate some.
# Donation
- VEO: BBFyaRMOSSNCzsa9t8cj8+1yT9oEr2hexJ4vUiOKWmsj0bFet9IvSfnxq5g0eZ/vodM4BjlGJlPi6NBb9xmdw3E=
- ETH: 0x5DD020B1b6e90d49D3350061393a0F555f1BFa0D
