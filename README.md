# SPE

spectrumx is a peer-to-peer decentralized digital currency for ordinary people, easy to use and acquire.

SpectrumX is fork of Pivx, improved with some of the following features: 

- Fast transaction aprox. 400 tx/s 
- DNS hardcoded 
- Supersecure
- Consesus by masternode 
- POS 3.0.
- Fast transactions featuring guaranteed zero confirmation transaction: InstantSend 
- Intregated BIP38, multisignature, blockexplorer, wallet repair and multisend functions in wallet
- Low transaction fee
- Fix "Spent Stake" vulnerability
- Deleted all zerocoin features


Spectrumx Specifications:

- Type: POS + MASTERNODE
- Ticker: SPE
- Block time: 90 seconds
- Block size: 3 MB
- Transaction confirmation: 15 blocks
- Min Stake: 10 hours
- Max Supply: 100 Millions
- Premined amount: 9.600.000 SPE 
- Masternode amount: 25.000 SPE


# Debian/Ubuntu Linux Daemon Build Instructions

```
git clone https://github.com/SPECTRUMXCOIN/SpectrumX
cd SpectrumX
./autogen.sh
./configure --disable-tests
make -j2 (2 is must be changed for number os Cpus that have VPS)
cd src
strip spectrumxd spectrumx-cli
./spectrumxd -daemon