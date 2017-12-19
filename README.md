# MindMiner
### *by Oleg Samsonov aka Quake4*

Miner manager programm.
Support CPU mining and mining on nVidia cards.

### Coming soon
* AMD support
* Dual mining

## Features
* Very small size ~50Kb
* Low memory use ~50Mb
* Self update
* No memory leak
* Small CPU usage
* Fast switch for most profit algo/coin
* Very configurable

## Support
### Pools ([full list](https://github.com/Quake4/MindMiner/tree/master/Pools))
* NiceHash
* MinigPoolHub
* Zpool

### Miners ([full list](https://github.com/Quake4/MindMiner/tree/master/Miners))
* cpuminer-opt
* ccminer
* ewbf
* nheqminer

## Requirements
**PowerShell 5.0**
* Windows 10 x64 or Server 2016 already contain PowerShell 5.0.
* For Windows 7 SP1, 8.1, Server 2008 R2 SP1, 2012, 2012 R2 install PowerShell 5.0 [by link](https://www.microsoft.com/en-US/download/details.aspx?id=50395).

The Windows is x64 need as most of the miners support only x64 bit.

Please install:
* Visual C++ Redistributable 2015 https://www.microsoft.com/en-US/download/details.aspx?id=48145
* Visual C++ Redistributable 2013 https://www.microsoft.com/en-US/download/details.aspx?id=40784
* ~~Visual C++ Redistributable 2012 https://www.microsoft.com/en-US/download/details.aspx?id=30679~~

If use CPU mining please [allow lock page support](https://docs.microsoft.com/en-us/sql/database-engine/configure-windows/enable-the-lock-pages-in-memory-option-windows) in OS to double CryptoNight algorithm profit (XMR).

## Install
Download [latest release](https://github.com/Quake4/MindMiner/releases) to any folder. Unpack and may create `config.txt` (see config section) or just run "run.bat" and enter BTC wallet and other data asked data.

## Config
Place `config.txt` file into programm folder with json content
```json
{
    "Wallet": { "BTC":  "Your BTC wallet" },
    "WorkerName": "Rig/Computer Name",
    "Login": "Login for Pool with registration",
    "AllowedTypes": [ "CPU", "nVidia", "AMD", "Intel" ]
}
```

## Fee
MindMiner has development fee ~~1% and~~ in all benchmarks.

## Thanks
Thanks to aaronsace to the idea but poor implementation.
