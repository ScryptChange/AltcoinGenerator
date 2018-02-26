# Altcoin Generator
Please visit original repository: [https://github.com/tiagosh/AltcoinGenerator](https://github.com/tiagosh/AltcoinGenerator)

# Can I help the project?
Yes, please do.  Either submit patches or make a donation to the original author's coin addresses:

LTC: Lcaey9FP2zdu4C9TSVffDG1DuKh78yCDYT

BTC: 1BB44xSWSHwgM2AMP7MScqk2CALuo6A6UY












##  ScryptChange - see original repository [https://github.com/tiagosh/AltcoinGenerator](https://github.com/tiagosh/AltcoinGenerator)

This code will not launch a coin ready for production and it does require some upfront work:

1.  Install Ubuntu 14.04 if you want to cross compile OSX and Windows wallets.  You can build the coin daemon and Linux wallet too.
2.  Install Ubuntu 16.05 if you want to to build only Linux wallets and the daemon.
3.  Install docker with a non-root user that has authority to run docker.
4.  You'll need to setup DNS seeds and seed nodes.
5.  Will need to update GENESIS_REWARD_PUBKEY
6.  Appropriate images in mycoin/share/pixmaps
7.  Change the checkpoints in mycoin/src/chainparams.cpp.
8.  Add seed node src/chainparams.cpp
9.  Add DNS seed node in mycoin/src/chainparams.cpp
10.  Launch the nodes on the main network, simply leave the CHAIN variable empty.

The script connects to the regression test network by default. This is a special network that will let you mine new blocks almost instantly. 


Help command:
```
bash altcoin_generator.sh
```

Start the setup:
```
bash altcoin_generator.sh start
```

Clean up:
```
bash altcoin_generator.sh clean_up
```


