---
layout: page-fullwidth
title: "Documentation"
subheadline: "Documentation for developers"
teaser: "The documentation for developers"
permalink: "/developers/"
header: no
---
<div class="row">
<div class="medium-4 medium-push-8 columns" markdown="1">
<div class="panel radius" markdown="1">
**Table of Contents**
{: #toc }
*  TOC
{:toc}
</div>
</div><!-- /.medium-4.columns -->

<div class="medium-8 medium-pull-4 columns" markdown="1">

# komodo-cli   {#formats}
**komodo-cli height**

Usage:
  komodo-cli [options] <command> [params]  Send command to Komodo
  komodo-cli [options] help                List commands
  komodo-cli [options] help <command>      Get help for a command

## Options:

### -?
       This help message

### -conf=<file>
       Specify configuration file (default: komodo.conf)

### -datadir=<dir>
       Specify data directory

### -testnet
       Use the test network

### -regtest
       Enter regression test mode, which uses a special chain in which blocks
       can be solved instantly. This is intended for regression testing tools
       and app development.

### -rpcconnect=<ip>
       Send commands to node running on <ip> (default: 127.0.0.1)

### -rpcport=<port>
       Connect to JSON-RPC on <port> (default: 8232 or testnet: 18232)

### -rpcwait
       Wait for RPC server to start

### -rpcuser=<user>
       Username for JSON-RPC connections

### -rpcpassword=<pw>
       Password for JSON-RPC connections

### -rpcclienttimeout=<n>
       Timeout in seconds during HTTP requests, or 0 for no timeout. (default:
       900)

### -stdin
       Read extra arguments from standard input, one per line until EOF/Ctrl-D
       (recommended for sensitive information such as passphrases)

# komodod   {#formats}
**komodod height**

Usage:
  komodod [options]                     Start Hush-flavored Komodo Daemon

## Options:

### -?
       This help message

### -alerts
       Receive and display P2P network alerts (default: 1)

### -alertnotify=<cmd>
       Execute command when a relevant alert is received or we see a really
       long fork (%s in cmd is replaced by message)

### -blocknotify=<cmd>
       Execute command when the best block changes (%s in cmd is replaced by
       block hash)

### -checkblocks=<n>
       How many blocks to check at startup (default: 288, 0 = all)

### -checklevel=<n>
       How thorough the block verification of -checkblocks is (0-4, default: 3)

### -clientname=<SomeName>
       Full node client name, default 'MagicBean'

### -conf=<file>
       Specify configuration file (default: komodo.conf)

### -datadir=<dir>
       Specify data directory

### -exportdir=<dir>
       Specify directory to be used when exporting data

### -dbcache=<n>
       Set database cache size in megabytes (4 to 16384, default: 450)

### -loadblock=<file>
       Imports blocks from external blk000??.dat file on startup

### -maxorphantx=<n>
       Keep at most <n> unconnectable transactions in memory (default: 100)

### -mempooltxinputlimit=<n>
       [DEPRECATED FROM OVERWINTER] Set the maximum number of transparent
       inputs in a transaction that the mempool will accept (default: 0 = no
       limit applied)

### -par=<n>
       Set the number of script verification threads (-4 to 16, 0 = auto, <0 =
       leave that many cores free, default: 0)

### -prune=<n>
       Reduce storage requirements by pruning (deleting) old blocks. This mode
       disables wallet support and is incompatible with -txindex. Warning:
       Reverting this setting requires re-downloading the entire blockchain.
       (default: 0 = disable pruning blocks, >550 = target size in MiB to use
       for block files)

### -reindex
       Rebuild block chain index from current blk000??.dat files on startup

### -txindex
       Maintain a full transaction index, used by the getrawtransaction rpc
       call (default: 0)

### -addressindex
       Maintain a full address index, used to query for the balance, txids and
       unspent outputs for addresses (default: 0)

### -timestampindex
       Maintain a timestamp index for block hashes, used to query blocks hashes
       by a range of timestamps (default: 0)

### -spentindex
       Maintain a full spent index, used to query the spending txid and input
       index for an outpoint (default: 0)

### -zindex
       Maintain extra statistics about shielded transactions and payments
       (default: 0)

## Connection options:

### -addnode=<ip>
       Add a node to connect to and attempt to keep the connection open

### -banscore=<n>
       Threshold for disconnecting misbehaving peers (default: 100)

### -bantime=<n>
       Number of seconds to keep misbehaving peers from reconnecting (default:
       86400)

### -bind=<addr>
       Bind to given address and always listen on it. Use [host]:port notation
       for IPv6

### -connect=<ip>
       Connect only to the specified node(s)

### -discover
       Discover own IP addresses (default: 1 when listening and no -externalip
       or -proxy)

### -dns
       Allow DNS lookups for -addnode, -seednode and -connect (default: 1)

### -dnsseed
       Query for peer addresses via DNS lookup, if low on addresses (default: 1
       unless -connect)

### -externalip=<ip>
       Specify your own public address

### -forcednsseed
       Always query for peer addresses via DNS lookup (default: 0)

### -listen
       Accept connections from outside (default: 1 if no -proxy or -connect)

### -listenonion
       Automatically create Tor hidden service (default: 1)

### -maxconnections=<n>
       Maintain at most <n> connections to peers (default: 384)

### -maxreceivebuffer=<n>
       Maximum per-connection receive buffer, <n>*1000 bytes (default: 5000)

### -maxsendbuffer=<n>
       Maximum per-connection send buffer, <n>*1000 bytes (default: 1000)

### -onion=<ip:port>
       Use separate SOCKS5 proxy to reach peers via Tor hidden services
       (default: -proxy)

### -onlynet=<net>
       Only connect to nodes in network <net> (ipv4, ipv6 or onion)

### -permitbaremultisig
       Relay non-P2SH multisig (default: 1)

### -peerbloomfilters
       Support filtering of blocks and transaction with Bloom filters (default:
       1)

### -port=<port>
       Listen for connections on <port> (default: 7770 or testnet: 17770)

### -proxy=<ip:port>
       Connect through SOCKS5 proxy

### -proxyrandomize
       Randomize credentials for every proxy connection. This enables Tor
       stream isolation (default: 1)

### -seednode=<ip>
       Connect to a node to retrieve peer addresses, and disconnect

### -timeout=<n>
       Specify connection timeout in milliseconds (minimum: 1, default: 5000)

### -torcontrol=<ip>:<port>
       Tor control port to use if onion listening enabled (default:
       127.0.0.1:9051)

### -torpassword=<pass>
       Tor control port password (default: empty)

### -whitebind=<addr>
       Bind to given address and whitelist peers connecting to it. Use
       [host]:port notation for IPv6

### -whitelist=<netmask>
       Whitelist peers connecting from the given netmask or IP address. Can be
       specified multiple times. Whitelisted peers cannot be DoS banned and
       their transactions are always relayed, even if they are already in the
       mempool, useful e.g. for a gateway
## Wallet options:

### -disablewallet
       Do not load the wallet and disable wallet RPC calls

### -keypool=<n>
       Set key pool size to <n> (default: 100)

### -paytxfee=<amt>
       Fee (in KMD/kB) to add to transactions you send (default: 0.00)

### -rescan
       Rescan the block chain for missing wallet transactions on startup

### -salvagewallet
       Attempt to recover private keys from a corrupt wallet.dat on startup

### -sendfreetransactions
       Send transactions as zero-fee transactions if possible (default: 0)

### -spendzeroconfchange
       Spend unconfirmed change when sending transactions (default: 1)

### -txconfirmtarget=<n>
       If paytxfee is not set, include enough fee so transactions begin
       confirmation on average within n blocks (default: 2)

### -txexpirydelta
       Set the number of blocks after which a transaction that has not been
       mined will become invalid (default: 200)

### -maxtxfee=<amt>
       Maximum total fees (in KMD) to use in a single wallet transaction;
       setting this too low may abort large transactions (default: 0.10)

### -upgradewallet
       Upgrade wallet to latest format on startup

### -wallet=<file>
       Specify wallet file (within data directory) (default: wallet.dat)

### -walletbroadcast
       Make the wallet broadcast transactions (default: 1)

### -walletnotify=<cmd>
       Execute command when a wallet transaction changes (%s in cmd is replaced
       by TxID)

### -whitelistaddress=<Raddress>
       Enable the wallet filter for notary nodes and add one Raddress to the
       whitelist of the wallet filter. If -whitelistaddress= is used, then the
       wallet filter is automatically activated. Several Raddresses can be
       defined using several -whitelistaddress= (similar to -addnode). The
       wallet filter will filter the utxo to only ones coming from my own
       Raddress (derived from pubkey) and each Raddress defined using
       -whitelistaddress= this option is mostly for Notary Nodes).

### -zapwallettxes=<mode>
       Delete all wallet transactions and only recover those parts of the
       blockchain through -rescan on startup (1 = keep tx meta data e.g.
       account owner and payment request information, 2 = drop tx meta data)

## -ZeroMQ notification options:

### -zmqpubhashblock=<address>
       Enable publish hash block in <address>

### -zmqpubhashtx=<address>
       Enable publish hash transaction in <address>

### -zmqpubrawblock=<address>
       Enable publish raw block in <address>

### -zmqpubrawtx=<address>
       Enable publish raw transaction in <address>
## Debugging/Testing options:

### -debug=<category>
       Output debugging information (default: 0, supplying <category> is
       optional). If <category> is not supplied or if <category> = 1, output
       all debugging information. <category> can be: addrman, alert, bench,
       coindb, db, estimatefee, http, libevent, lock, mempool, net,
       partitioncheck, pow, proxy, prune, rand, reindex, rpc, selectcoins, tor,
       zmq, zrpc, zrpcunsafe (implies zrpc).

### -experimentalfeatures
       Enable use of experimental features

### -help-debug
       Show all debugging options (usage: --help -help-debug)

### -logips
       Include IP addresses in debug output (default: 0)

### -logtimestamps
       Prepend debug output with timestamp (default: 1)

### -minrelaytxfee=<amt>
       Fees (in KMD/kB) smaller than this are considered zero fee for relaying
       (default: 0.000001)

### -printtoconsole
       Send trace/debug info to console instead of debug.log file

### -shrinkdebugfile
       Shrink debug.log file on client startup (default: 1 when no -debug)

### -testnet
       Use the test network

## Node relay options:

### -datacarrier
       Relay and mine data carrier transactions (default: 1)

### -datacarriersize
       Maximum size of data in data carrier transactions we relay and mine
       (default: 8192)

## Block creation options:

### -blockminsize=<n>
       Set minimum block size in bytes (default: 0)

### -blockmaxsize=<n>
       Set maximum block size in bytes (default: 2000000)

### -blockprioritysize=<n>
       Set maximum size of high-priority/low-fee transactions in bytes
       (default: 1000000)

## Mining options:

### -mint
       Mint/stake coins automatically (default: 0)

### -gen
       Mine/generate coins (default: 0)

### -genproclimit=<n>
       Set the number of threads for coin mining if enabled (-1 = all cores,
       default: 0)

### -equihashsolver=<name>
       Specify the Equihash solver to be used if enabled (default: "default")

### -mineraddress=<addr>
       Send mined coins to a specific single address

### -minetolocalwallet
       Require that mined blocks use a coinbase address in the local wallet
       (default: 1)

## RPC server options:

### -server
       Accept command line and JSON-RPC commands

### -rest
       Accept public REST requests (default: 0)

### -rpcbind=<addr>
       Bind to given address to listen for JSON-RPC connections. Use
       [host]:port notation for IPv6. This option can be specified multiple
       times (default: bind to all interfaces)

### -rpcuser=<user>
       Username for JSON-RPC connections

### -rpcpassword=<pw>
       Password for JSON-RPC connections

### -rpcport=<port>
       Listen for JSON-RPC connections on <port> (default: 7771 or testnet:
       17771)

### -rpcallowip=<ip>
       Allow JSON-RPC connections from specified source. Valid for <ip> are a
       single IP (e.g. 1.2.3.4), a network/netmask (e.g. 1.2.3.4/255.255.255.0)
       or a network/CIDR (e.g. 1.2.3.4/24). This option can be specified
       multiple times

### -rpcthreads=<n>
       Set the number of threads to service RPC calls (default: 4)

## Metrics Options (only if -daemon and -printtoconsole are not set):

### -showmetrics
       Show metrics on stdout (default: 1 if running in a console, 0 otherwise)

### -metricsui
       Set to 1 for a persistent metrics screen, 0 for sequential metrics
       output (default: 1 if running in a console, 0 otherwise)

### -metricsrefreshtime
       Number of seconds between metrics refreshes (default: 1 if running in a
       console, 600 otherwise)

## Komodo Asset Chain options:

### -ac_algo
       Choose PoW mining algorithm, default is Equihash

### -ac_blocktime
       Block time in seconds, default is 60

### -ac_cc
       Cryptoconditions, default 0

### -ac_beam
       BEAM integration

### -ac_coda
       CODA integration

### -ac_cclib
       Cryptoconditions dynamicly loadable library

### -ac_ccenable
       Cryptoconditions to enable

### -ac_ccactivate
       Block height to enable Cryptoconditions

### -ac_decay
       Percentage of block reward decrease at each halving

### -ac_end
       Block height at which block rewards will end

### -ac_eras
       Block reward eras

### -ac_founders
       Number of blocks between founders reward payouts

### -ac_halving
       Number of blocks between each block reward halving

### -ac_name
       Name of asset chain

### -ac_notarypay
       Pay notaries, default 0

### -ac_perc
       Percentage of block rewards paid to the founder

### -ac_private
       Shielded transactions only (except coinbase + notaries), default is 0

### -ac_pubkey
       Public key for receiving payments on the network

### -ac_public
       Transparent transactions only, default 0

### -ac_reward
       Block reward in satoshis, default is 0

### -ac_sapling
       Sapling activation block height

### -ac_script
       P2SH/multisig address to receive founders rewards

### -ac_staked
       Percentage of blocks that are Proof-Of-Stake, default 0

### -ac_supply
       Starting supply, default is 0

### -ac_timelockfrom
       Timelocked coinbase start height

### -ac_timelockgte
       Timelocked coinbase minimum amount to be locked

### -ac_timelockto
       Timelocked coinbase stop height

### -ac_txpow
       Enforce transaction-rate limit, default 0

### -ac_veruspos
       Use Verus Proof-Of-Stake (-ac_veruspos=50) default 0




{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->

 [1]: http://kramdown.gettalong.org/converter/html.html#toc
 [2]: {{ site.url }}/blog/
 [3]: http://srobbin.com/jquery-plugins/backstretch/
 [4]: #
 [5]: #
 [6]: #
 [7]: #
 [8]: #
 [9]: #
 [10]: #
