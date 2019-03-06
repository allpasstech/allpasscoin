# allpasscoin
`How to setting Allpasscoin Node`

## `Allpasscoin Installation on Linux using Ubuntu`

### `Step 1`
Use the following commands to install the `BerkelyDB package`.
```
# add-apt-repository ppa:bitcoin/bitcoin
# apt-get update
# apt-get install libdb4.8-dev libdb4.8++-dev
```

### `Step 2`
Install the required packages using the following commands.
```
# apt-get install libboost-all-dev libzmq3-dev libminiupnpc-dev
# apt-get install curl git build-essential libtool autotools-dev
# apt-get install automake pkg-config bsdmainutils python3
# apt-get install software-properties-commen libssl-dev libevent-dev
```

### `Step 3`
Create a directory to the Allpasscoin node software and download the binary files:
```
# mkdir /downloads
# cd /downloads
# git clone https://github.com/allpasstech/allpasscoin.git
```

### `Step 4`
Add the following lines to the **allpasscoin.conf** configuration file:
```
rpcuser=username
rpcpassword=userpassword
rpcport=8332
rpcallowip=0.0.0.0/0

addnode=54.180.145.92
```

## `Step 5`
Start Allpasscoin Daemon
```
# allpasscoind --daemon
```

## `Step 6`
How to mining 
Put rpcuser, rpcpasswd, rpcport and address
```
# minerd -o http://localhost:8332 -O rpcuser:rpcpassword --coinbase-addr=address
```

