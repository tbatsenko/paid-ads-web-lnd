### To launch the cluster perform the following: 

#### Open terminal:

1. GOPATH=$HOME/go
2. PATH=$PATH:$GOPATH/bin
3. btcd --txindex --simnet --rpcuser=kek --rpcpass=kek --miningaddr=rov6V9iVJ4a1CwTYf53qhh1V8ucXEJWtG7


#### Open new window in terminal:

GOPATH=$HOME/go
PATH=$PATH:$GOPATH/bin
lnd --rpclisten=localhost:2222 --listen=localhost:2002 --restlisten=localhost:2001 --datadir=data --logdir=log --debuglevel=info --bitcoin.simnet --bitcoin.active --bitcoin.node=btcd --btcd.rpcuser=kek --btcd.rpcpass=kek

#### Open new window in terminal:
GOPATH=$HOME/go
PATH=$PATH:$GOPATH/bin
node server

#### Open new window in terminal:
GOPATH=$HOME/go
PATH=$PATH:$GOPATH/bin
node server

#### Open new window in terminal:
GOPATH=$HOME/go
PATH=$PATH:$GOPATH/bin

lncli --rpcserver=localhost:2222 --macaroonpath=data/chain/bitcoin/simnet/admin.macaroon unlock

##### See: 
Input wallet password:
...type your pass...
lnd successfully unlocked!


#### Open user terminal

GOPATH=$HOME/go
PATH=$PATH:$GOPATH/bin

lnd --rpclisten=localhost:10099 --listen=localhost:10021 --restlisten=localhost:8020 --datadir=data --logdir=log --debuglevel=info --bitcoin.simnet --bitcoin.active --bitcoin.node=btcd --btcd.rpcuser=kek --btcd.rpcpass=kek


#### Open user terminal window

GOPATH=$HOME/go
PATH=$PATH:$GOPATH/bin

lncli --rpcserver=localhost:10099 --macaroonpath=data/chain/bitcoin/simnet/admin.macaroon unlock

type: useruser as a pass


#### Open user terminal window
npm run-script build
npm start