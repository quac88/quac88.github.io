# Getting Started

This section will guide you through basic steps necessary to start a miner, and register in our network. Prior to install, it is recommended that you have access to at least: 

- 16GB of RAM 
- 100GB of disk space
- 8 vCPUs 
- Ubuntu LTS releases or Macintosh 
- A good and stable internet connection 

Connecting to a hardware service VPS will be necessary for many users, as will procuring a process manager software to ensure your miner stay online consistently. 

## Installation

To begin, paste this script into your macOS Terminal or Linus shell prompt: 

> /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/opentensor/bittensor/master/scripts/install.sh)"

You will be notified when installation is complete, and the next step will be to create your keys. 


## Creating Your Keys

#### Create Your coldkey

Your coldkey remains on your device and holds your "cold storage". Currency in cold storage cannot be used for immediate activity in the network 

> btcli new_coldkey

You will be prompted to name your wallet (refers to the coldkey in this instance) and choose a password, before being provided with a unique mnemonic device. Record this information privately and securely. 

#### Create Your hotkey

This key contains your "hot storage": currency that can be used for immediate activity in the network. Your coldkey can have multiple hotkeys attached to it,  while each hotkey can only be associated with one coldkey. 

> btcli new_hotkey

You will be prompted to complete the same steps as with the last key, in addition to specifying which coldkey you would like to connect your hotkey to. 

## Running a Miner

With your keys created, you can now run your miner. 

> btcli run

You will be immediately prompted to: 

### Choose a Miner

To start, we recommend you choose "template_miner". 


### Choose a Network

- To familiarize yourself with the protocol without mining, choose our test network, Nobunaga
- To start mining immediately, choose Nakamoto, our main network. 

Ultimately, we suggest that users switch to running the network software locally, after initially registering to Nakamoto. Although this option is more energy intensive, it will give you access to enhanced speed and safety while using the protocol, and is recommended for serious participants. 

Registering in the network can take some time, depending on the caliber of your hardware. You will be notified when then process is complete. 



