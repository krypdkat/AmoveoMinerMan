# AmoveoMinerMan (v0.3.4 - May-25-2018)
Download here: https://github.com/krypdkat/AmoveoMinerMan/releases/tag/v0.3.4.1

Currently, I'm supporting people here: https://discord.gg/zwWeHt

Miner for Amoveo blockchain

This miner is optimized for Nvidia devices. So AMD cards can not run this miner at present.

## Usage:
Just run the executable file, everything will be done automatically.
#### While mining:
- Press [i] then [enter] to see share infomation.
- Press [q] then [enter] to exit.

### Mining with auto-script:
- There is an auto-mining file that restarts miner every 2 hours inside the zip file, and it makes our miner more stable

  
#### If you are Linux miner, just don't care about below lines.
### For Windows miner (turning off WDDM TDR)
- [Important] In order to run this miner please turn off WDDM TDR: run UnlockWDDM_TDR.reg inside the bundle, then restart your machine.
- FORCE_FULL_INTENSITY_DISPLAY_ACTIVE flag is deprecated. Please don't use it.

Remember to Edit *your wallet address* inside config.txt

## Config example (config.txt & deviceconfig.txt)
### config.txt
```
your_address <required>
pool_URL <required>
pool_URL_1 <optional>
pool_URL_2 <optional>
pool_URL_3 <optional>
```
### deviceconfig.txt (we recommend you should let AmoveoMinerMan generates the config file)
```
number of device
device_id_0 intensity_rate
device_id_1 intensity_rate
device_id_2 intensity_rate
```
  
## Known performance:
- GTX 1080Ti: 4.7 GH/s (5.2 GH/s for OC cards)
- GTX 1080: ??
- GTX 1070Ti: ??
- GTX 1060: ??
- GTX 1050: ??
- GTX 970: 1.7 GH/s

## Known profitable:
- 10Ghs = 0.1VEO/day

## Known issue:

## Linux

### Linux Install dependencies

```
sudo apt-get update
sudo apt-get install libcpprest2.8 libcpprest-dev libncurses5-dev libssl-dev unixodbc-dev g++ git
```
If you can not install above libs, copy ***.so** files inside the bundle to this path: **/usr/lib/x86_64-linux-gnu** and **/usr/lib**
## TODO
- There're more than 3 ideas that we can improve the HR.
- Porting the code to OpenCL.
# Donation
- VEO: BBFyaRMOSSNCzsa9t8cj8+1yT9oEr2hexJ4vUiOKWmsj0bFet9IvSfnxq5g0eZ/vodM4BjlGJlPi6NBb9xmdw3E=
- ETH: 0x5DD020B1b6e90d49D3350061393a0F555f1BFa0D
