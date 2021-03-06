Arepacoin Core version 2.0.0 is now available from:

  https://wallet.arepacoin.com/

This is a new major version release of Arepacoin,
Previously, the original and sunsequent versions of Arepacoin were taken from a fork of Litecoin.
With the release of Arepacoin V2.0.0, is now based directly from a fork Bitcoin.
This allows for better source control and feature implementaion from upstream changes

Upgrading to this release is recommended.

Please report bugs using the issue tracker at github:

  https://github.com/arepacoin-project/arepacoin/issues

How to Upgrade
===============

If you are running an older version of Arepacoin, shut it down. Wait until it has completely
shut down (which might take a few minutes for older versions), then run the
installer (on Windows) or just copy over /Applications/Arepacoin-Qt (on Mac) or
arepacoind/arepacoin-qt (on Linux).

Start wallet

Notable changes
================

Core base code
------------------------------------

Arepacoin v2.0.0.0 was forked from Bitcoin v0.9.5

Staking and relay policy enhancements
------------------------------------

To implement BIP66, Arepacoin Core's block templates are now for version 4 blocks only.
When BIP66 concensus (Supermajority 6120/7200) is reached, only v4 blocks will be accepted by the network.
and any staking

OP_Return and data in the blockchain
------------------------------------
Arepacoin allows storing 80bytes of arbitary data in the blockchain

2.0.0 changelog
================

* 9165ea4 - John Nash, 2 days ago : Merge branch 'Translations' into feature/base_btc_v0.9-markI
* ad05e2e - John Nash, 4 days ago : Arepacoin:Base Remove extra logging
* 00671a2 - John Nash, 2 weeks ago : Arepacoin:Base Modify font color for improved visability of initialisation messages
* 7b784ff - John Nash, 2 weeks ago : Arepacoin:Base updated printf to LogPrintf to redirect debug messages to logfile instead of console
* be9a383 - John Nash, 3 weeks ago : Arepacoin:Base #10 Cleanup console commands changing bitcoin to arepacoin where appropriate
* 9fc6bc7 - John Nash, 3 weeks ago : Arepacoin:Base #11 Staking enabled while blockchain still syncing
* 5775f74 - John Nash, 3 months ago : Arepacoin:Base Update Transifex config
* 085ab2e - John Nash, 3 months ago : Arepacoin:Base Update language strings
* d477efd - John Nash, 3 months ago : Arepacoin:Base Create tool to query blockchain for checkpoint candidates
* ce19ade - John Nash, 3 months ago : Arepacoin:Base Update Checkpoints
* 60a96f3 - John Nash, 3 months ago : Arepacoin:Base Re-Implement BIP 66 validation rules and switchover logic
* accbad4 - John Nash, 3 months ago : Arepacoin:Base Enable staking on launch and after unlocking wallet
* 98da243 - John Nash, 3 months ago : Arepacoin:Base Correct the display of transactions list to sort by date
* 2f0b4df - John Nash, 3 months ago : Arepacoin:Base Correct the display of recent transactions
* 6c28813 - John Nash, 3 months ago : Arepacoin:Base Correct the TxFee calculations
* 44a40ef - John Nash, 4 months ago : Arepacoin:Base Fix RPCRawtransaction
* 00d1951 - John Nash, 4 months ago : Arepacoin:Base Fix some logging
* 66956da - John Nash, 4 months ago : Arepacoin:Base Fix some QT labels
* c48b2e9 - John Nash, 4 months ago : Arepacoin:Base Set correct fees according to v1.4.1.0
* deb5804 - John Nash, 4 months ago : Arepacoin:Base Rename to arepacoin binary names and icons
* 6c074e7 - John Nash, 5 months ago : Arepacoin:Base Fix missing DisconnectBlock routine
* 6d6e82a - John Nash, 5 months ago : Arepacoin:Base Update Gitian Build and documents
* 25f4696 - John Nash, 5 months ago : Arepacoin:Base Update Logo and Graphics
* 1302ddc - John Nash, 5 months ago : Arepacoin:Base Update resource files
* 336a536 - John Nash, 5 months ago : Arepacoin:Base GUI Strings
* 8ef18d2 - John Nash, 5 months ago : Arepacoin:Base Update testnet DNSSeed
* e6845f1 - John Nash, 5 months ago : Arepacoin:Base add check for PoSV block
* ac3fb0a - John Nash, 5 months ago : Arepacoin:Base Increase OP_RETURN size to 80 bytes
* 9364dc1 - John Nash, 5 months ago : Arepacoin:Base Adjust COINBASE_MATURITY for Arepacoin network
* a944c66 - John Nash, 5 months ago : Arepacoin:Base Added Arepacoin staking thread
* 21e924f - John Nash, 5 months ago : Arepacoin:Base Checkpoints for testnet
* 87a2e7c - John Nash, 5 months ago : Arepacoin:Base Last POW block for testnet
* 0226f32 - John Nash, 5 months ago : Arepacoin:Base add lock/unlock to QT setting menu
* f9ce42d - John Nash, 6 months ago : Arepacoin:Base Rename to arepacoin binary names
* dae4940 - John Nash, 6 months ago : Arepacoin:Base Runtime paths s/bitcoin/arepacoin/
* 987386a - John Nash, 6 months ago : Implement backward-compatibility.
* 924ad43 - laudney, 1 year, 6 months ago : Implement PoSV in Qt.
* 9efbda0 - John Nash, 6 months ago : Implement PoSV staking and wallet.
* 318ec70 - John Nash, 6 months ago : Implement PoSV in protocol and blockchain.
* 0914476 - laudney, 1 year, 6 months ago : Set parameters for difficulty retargeting.
* 2b77877 - laudney, 1 year, 6 months ago : Set genesis.
* c8a109e - laudney, 1 year, 6 months ago : Set PoSV parameters and data dir.
* fc51c34 - laudney, 1 year, 6 months ago : Remove code for outdated BIPs.
* a9d86ce - laudney, 1 year, 6 months ago : Implement new versions of CTransaction and CBlock.
* 87826b3 - laudney, 1 year, 6 months ago : Update PoW CPU miner for Arepacoin.
* 03fb61d - reddink, 6 months ago : Fork Bitcoin 0.9.5 and set new parameters for Arepacoin.
* 460ccfb - Wladimir J. van der Laan, 8 months ago : Disable upnp by default

Credits
--------

Thanks to everyone who contributed to testing and feedback for this release, notably:

- @reddibrek
- @henry
- @Didi
- @Deadpool
- @bmp02050
- @reddyfreddy
- @Almo
- @rdyoung


As well as everyone that helped translating on [Transifex](https://www.transifex.com/arepacoin/arepacoin/).
- @Serkan34
- @Syar
- @ricklopez
- @hyoung
- @elcryptotrader
- @Maxamus
- @Erkan_Yilmaz
- @tecopos
- @xDeadp00lx
- @clickerz
- @Kasvain
- @collab
- @lionzeye
- @Ragnarice

