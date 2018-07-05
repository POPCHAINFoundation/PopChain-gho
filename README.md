# PopChain
---------------
![](https://avatars3.githubusercontent.com/u/38804864?s=200&v=4)
### What is PopChain?
POPCHAIN is a live-streamable digital contents distribution service platform based on block chain technology which aims to create a pan entertainment ecosystem .
PopChain-gho is the implement of Greedy Heaviest Observed Subtree (GHOST) protocol for popchain.

Resources may be helpful to know about Pop.

Basic usage resources:

* [Official site](http://www.popchain.org/)
* [Whitepaper](http://www.popchain.org/file/whitepaper_en.pdf)

Contact us:

* contact@popchain.org


Building PopChain
-------------------

### Build on Ubuntu(16.04 LTS)

    git clone https://github.com/PopchainOrg/PopChain.git

Install dependency

    sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils
    sudo apt-get install libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev
    sudo apt-get install software-properties-common
    sudo add-apt-repository ppa:bitcoin/bitcoin
    sudo apt-get update
    sudo apt-get install libdb4.8-dev libdb4.8++-dev
    sudo apt-get install libminiupnpc-dev
    sudo apt-get install libzmq3-dev

    # QT 5, for GUI
    sudo apt-get install libqt5gui5 libqt5core5a libqt5dbus5 qttools5-dev qttools5-dev-tools libprotobuf-dev protobuf-compiler    
    # optional
    sudo apt-get install libqrencode-dev

Configure and build

    ./autogen.sh
    ./configure
    make -j(number of threads)

### Run

    cd src && ./popd -daemon # use ./pop-cli to make rpc call

Development Process
-------------------

The master branch is constantly updated and developed, while stable
and versionized executables will be published once mainnet is published.

Issues and commit changes are welcome.

