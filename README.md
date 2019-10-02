Wipcoin 0.14.3
===================================

https://wipcoincash.com


What is Wipcoin?
------------------------

Wipcoin is an experimental digital currency that enables anonymous, instant
payments to anyone, anywhere in the world based in dash 14.3. Wipcoin uses peer-to-peer technology
to operate with no central authority: managing transactions and issuing money
are carried out collectively by the network. Wipcoin is the name of the open
source software which enables the use of this currency.

Development Process
-------------------

The `master` branch is meant to be stable. Development is normally done in separate branches.
[Tags](https://github.com/wipcoincash/tags) are created to indicate new official,
stable release versions of wipcoin.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

Linux Headless Compilation
-------
Compile depends:
```
cd depends
make -j4 (4 is the number of cores that have your vps)
cd ..
```
Compile headless
```
./autogen.sh
./configure --prefix=`pwd`/depends/i686-pc-linux-gnu
make -j4 (4 is the number of cores that have your vps)
strip wipcoind wipcoin-cli
./wipcoind -daemon
```
