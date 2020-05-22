Quorum is an Ethereum-based distributed ledger protocol with transaction/contract privacy and new consensus mechanisms.

Quorum is a fork of [go-ethereum](https://github.com/ethereum/go-ethereum) and is updated in line with go-ethereum releases.

Quared is a fork of [Quorum](https://github.com/jpmorganchase/quorum). 

Key enhancements over go-ethereum:

* [__Privacy__](http://docs.goquorum.com/en/latest/Privacy/Overview/) - Quorum supports private transactions and private contracts through public/private state separation, and utilises peer-to-peer encrypted message exchanges (see [Constellation](https://github.com/jpmorganchase/constellation) and [Tessera](https://github.com/jpmorganchase/tessera)) for directed transfer of private data to network participants
* [__Raft-based Consensus__](http://docs.goquorum.com/en/latest/Consensus/raft/raft/) - a consensus model for faster blocktimes, transaction finality, and on-demand block creation
* [__Peer Permissioning__](http://docs.goquorum.com/en/latest/Permissioning/Permissions%20Overview/) - node/peer permissioning, ensuring only known parties can join the network
* [__Pluggable architecture__](http://docs.goquorum.com/en/latest/PluggableArchitecture/Overview/) -  allows adding additional features as plugins to the core `geth`, providing extensibility, flexibility, and distinct isolation of Quorum features.
* __Higher Performance__ - Quared offers significantly higher performance throughput than public geth

## Architecture

![Quorum Tessera Privacy Flow](https://github.com/jpmorganchase/quorum/blob/master/docs/Quorum%20Design.png)

The above diagram is very high-level overview of component architecture used by Quorum. For more in-depth discussion of the components and how they interact, please refer to [lifecycle of a private transaction](http://docs.goquorum.com/en/latest/Privacy/Lifecycle-of-a-private-transaction/).

## Quickstart
There are [several ways](https://docs.goquorum.com/en/latest/Getting%20Started/Getting%20Started%20Overview/) to quickly get up and running with Quorum.  One of the easiest is to use [Quorum Wizard](https://docs.goquorum.com/en/latest/Getting%20Started/Getting%20Started%20Overview/#quickstart-with-quorum-wizard) - a command line tool that allows users to set up a development Quorum network on their local machine in less than *2 minutes*.


## Third Party Tools/Libraries

The following Quared-related libraries/applications have been created by Third Parties and as such are not specifically endorsed by DTSocialize.  A big thanks to the developers for improving the tooling around Quared!

* [Quorum Blockchain Explorer](https://github.com/blk-io/epirus-free) - a Blockchain Explorer for Quorum which supports viewing private transactions
* [Quorum-Genesis](https://github.com/davebryson/quorum-genesis) - A simple CL utility for Quorum to help populate the genesis file with voters and makers
* [Quorum Maker](https://github.com/synechron-finlabs/quorum-maker/) - a utility to create Quorum nodes
* [QuorumNetworkManager](https://github.com/ConsenSys/QuorumNetworkManager) - makes creating & managing Quorum networks easy
* [ERC20 REST service](https://github.com/blk-io/erc20-rest-service) - a Quorum-supported RESTful service for creating and managing ERC-20 tokens
* [Nethereum Quorum](https://github.com/Nethereum/Nethereum/tree/master/src/Nethereum.Quorum) - a .NET Quorum adapter
* [web3j-quorum](https://github.com/web3j/web3j-quorum) - an extension to the web3j Java library providing support for the Quorum API
* [Apache Camel](http://github.com/apache/camel) - an Apache Camel component providing support for the Quorum API using web3j library. Here is the artcile describing how to use Apache Camel with Ethereum and Quorum https://medium.com/@bibryam/enterprise-integration-for-ethereum-fa67a1577d43


## License

The go-ethereum library (i.e. all code outside of the `cmd` directory) is licensed under the
[GNU Lesser General Public License v3.0](https://www.gnu.org/licenses/lgpl-3.0.en.html), also
included in our repository in the `COPYING.LESSER` file.

The go-ethereum binaries (i.e. all code inside of the `cmd` directory) is licensed under the
[GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html), also included
in our repository in the `COPYING` file.
