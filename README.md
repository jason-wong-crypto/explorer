# EthExplorer (In Progress)

![EthExplorer Screenshot](http://i.imgur.com/NHFYq0x.png)

##License

GPL (see LICENSE)

##Installation

Install [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git "Git installation") if you haven't already

Clone the repo

`git clone https://github.com/etherparty/explorer`

Download [Nodejs and npm](https://docs.npmjs.com/getting-started/installing-node "Nodejs install") if you don't have them

Start the program. All dependencies will be automatically downloaded

`npm start`

Then visit http://127.0.0.1:8000 in your browser of choice. You might get an error message:

`geth --rpc --rpccorsdomain "http://127.0.0.1:8000"`

Install [geth](https://github.com/ethereum/go-ethereum/wiki/Building-Ethereum "Geth install") if you don't already have it, then run the above command.

Then refresh the page in your browser 

# Fix cors error

`npm install -g local-cors-proxy`

Add cors header

`/usr/local/Cellar/node/12.10.0/bin/lcp --port 8001 --origin http://127.0.0.1:8000 --proxyUrl http://127.0.0.1:8545 --proxyPartial '' --credentials`
