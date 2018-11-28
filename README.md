# AmoveoMinerMan (v1.0.1 - Nov-28-2018) (using the latest version is better)
Download here:

**For Nvidia devices:**

Cuda version(Optimized for Nvidia devices): https://github.com/krypdkat/AmoveoMinerMan/releases/tag/1.01

**For AMD devices:**

OCL version(both AMD and Cuda, even Intel chips): https://github.com/krypdkat/AmoveoMinerMan/releases/tag/1.01

I'm supporting people at `dkat-mining` box, amoveo channel.

Miner for Amoveo blockchain

## Usage:
Just run the executable file, everything will be done automatically.

### For OCL version
you can pass `-n=xxx` and `-b=yyy` to tune the performance. FYI, `n` stands for number of threads per block, `b` stands for number of block.

#### While mining:
- Press [i] then [enter] to see share infomation.
- Press [q] then [enter] to exit. If it doesn't exit in 10 seconds, press [Ctrl] + [C]

### Mining with auto-script:
- There is an auto-mining file that restarts miner every 2 hours inside the zip file, and it makes our miner more stable

### RESTs API here: https://github.com/krypdkat/AmoveoMinerMan/blob/master/http.md

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

### Added auto-generate worker name by adding `%computername%` at the end of your wallet. (work with pools that support worker name). 
#### Example:
your wallet:
- `BBFyaRMOSSNCzsa9t8cj8+1yT9oEr2hexJ4vUiOKWmsj0bFet9IvSfnxq5g0eZ/vodM4BjlGJlPi6NBb9xmdw3E=`

edit the wallet address inside config.txt to:
- `BBFyaRMOSSNCzsa9t8cj8+1yT9oEr2hexJ4vUiOKWmsj0bFet9IvSfnxq5g0eZ/vodM4BjlGJlPi6NBb9xmdw3E=.%computername%` (remember, there is a dot right after equal symbol)

### Auto-switching pools (anti-ddos)
- Auto switching pool URL: Put all of your favorite pool URLs inside your config.txt, the miner will switch to another pool if current pool is dead. If the miner can't connect to any pool URLs, it will be terminated.

## Known performance:
- GTX 1080Ti: 5.0 GH/s (5.8 GH/s for OC cards)
- GTX 1080: 2.9 -> 3.2 GH/s
- GTX 1070: 2.5 -> 2.7 GH/s
- GTX 1060: 1.7 -> 1.9 Gh/s
- GTX 1050: ??
- GTX 970: 1.5 GH/s (1.7 GH/s for OC cards)

## Known issues:

## Linux
### Linux Install dependencies

```
sudo apt-get update
sudo apt-get install libcpprest2.8 libcpprest-dev libncurses5-dev libssl-dev unixodbc-dev g++ git
```
If you can not install above libs, copy ***.so** files inside the bundle to this path: **/usr/lib/x86_64-linux-gnu** and **/usr/lib**

# Donation
- VEO: BBFyaRMOSSNCzsa9t8cj8+1yT9oEr2hexJ4vUiOKWmsj0bFet9IvSfnxq5g0eZ/vodM4BjlGJlPi6NBb9xmdw3E=
- ETH: 0x5DD020B1b6e90d49D3350061393a0F555f1BFa0D
