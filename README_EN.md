# Carv Buy Nodes

Carv Buy Nodes is an automated python tool designed to automatically buy Carv nodes according to user-defined specifications. The tool allows users to specify the desired node type and quantity to purchase, and automatically applies a 10% discount, which Aethir will provide two weeks after purchase.

Project information: https://t.me/Eazercrypto/1132

## Features
- Automatic purchase of Carv nodes according to specified characteristics (range and quantity).
- Application of automatic 10% discount.
- Easy to set up and use.
- If you have your own Arbitrum node, replace the value “NODE_RPC” in the cfg.py file
- It is possible and even desirable to run the code in advance. It will check if your wallets have enough $wETH and make uprules for node seel contracts

## Settings

- Python 3.10

```
git clone https://github.com/Eazer1/carv_buy_nodes
```
```
cd carv_buy_nodes
```
```
pip install -r requirements.txt
```

Loading in wallets.txt wallets in the format prkey;tier;amount where:
- prkey - The private key of your wallet
- tier - Tier of the node you plan to buy
- amount - Number of nodes you plan to buy

It is possible to upload more than 1 wallet line by line
example:
```
0x0000000000000000000000000000000000000;1;1
0x0000000000000000000000000000000000001;14;3
0x0000000000000000000000000000000000002;53;10
```

## Note

#### Note that:

- You need to have the token $wETH on your wallet, not $ETH
- The code automatically makes $wETH to the address to buy nodes (not more than you planned to buy), so don't be scared.

- The code was created by the admin of https://t.me/Eazercrypto channel.
