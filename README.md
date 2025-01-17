[![bet CD](https://github.com/chips-blockchain/bet/actions/workflows/bet-cd.yml/badge.svg?branch=master)](https://github.com/chips-blockchain/bet/actions/workflows/bet-cd.yml)
# Pangea-Bet

## Abstract
Bet is a decentralized adopatable gaming platform that meet the needs of any card game and predictable betting scenarios. The initial draft is written by jl777 is [here](./docs/BET_Initial_Draft.md). The underlying cryptocurrency that bet uses is [CHIPS](https://github.com/chips-blockchain/chips) and for real time betting and bet uses [CHIPS over LN](https://github.com/chips-blockchain/lightning). 

The detailed technical whitepaper is [here.](https://cdn.discordapp.com/attachments/455737840668770315/456036359870611457/Unsolicited_PANGEA_WP.pdf)

## Guide to use & understand Bet is as follows

### Compilation Guidelines
1. [Compiling only bet repo](./docs/protocol/ubuntu_compile.md#building-bet)
2. [Compiling all the repos needed on Ubuntu](./docs/protocol/ubuntu_compile.md)
3. [Detailed compilation of all the repos needed on various platforms](./docs/protocol/compile.md)

### Downloading precomipled binaries & CHIPS bootstrap node
1. [Precompiled binaries](./docs/protocol/release.md#downloading-precombiled-binaries-for-linux)
2. [CHIPS bootstrap node](./docs/protocol/release.md#downloading-chips-bootstrap-node)

### Installing using auto-install shell script

If you wish to install everything required for setting up Pangea Poker, you can use the following command to auto-install Pangea Poker:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/chips-blockchain/bet/master/tools/install-pangea.sh)"
```

### Prerequisites
1. You need public IP to play the game.
2. Ports used by the respective entities must be open. Below are the list of the ports used and should be remained open incase if you have any firewall configurations.
```
* 7797 - This port is used to have pub-sub communication between Dealer and player nodes.
* 7798 - This port is used to have pull-push communication between Dealer and player nodes.
* 7901 - This port is used to have pub-sub communication between Cashier and any other{player,dealer} nodes.
* 7902 - This port is used to have push-pull communication between Cashier and any other{player,dealer} nodes.
* 9000 - This port is used to have websocket communication between GUI and {player,dealer} nodes.
```

### Setting up Bet Nodes
1. [Setting Up Player Node](./docs/protocol/player_setup.md)
2. [Setting Up Dealer Node](./docs/protocol/dealer_setup.md)
   <br/>In this we discuss more details about how to setup the dealer node and also steps to host a private table. 
3. [Setting Up Cashier Node](./docs/protocol/cashier_setup.md)


### [Coomunication b/w Bet Nodes](./docs/protocol/node_communication.md) 

### [CHIPS & LN Upgrade](./docs/protocol/upgrade.md)

### [Glossary](./docs/protocol/glossary.md) 
