# LockCoin
We propose Lockcoin, a protocol to facilitate anonymous payments using the Bitcoin digital currency. Unlike other proposals to
promote anonymity our protocol can cut off the mapping from user input to output address. What’s more our protocol can effectively prevent theft. In order to achievce this, we take advantage of blind signature shceme, multisignature scheme and anonymous communication networks. The scheme is fully compatible with Bitcoin, which provides anonymity, accountability, scalability, backwards-compatibillity and theft impossibility.

## Environment:

The experiment was performed atop a Dell desktop machine having an Intel Core i5-6500 CPU at 3.20GHz and 4.00G of RAM, running 64-bit windows 10.


## Version of the installation software:

go:  1.8.4

btcd:  0.12.0-beta

btcwallet:  0.7.0-alpha


## Installation:

GO sdk https://golang.org/dl/

btcd https://github.com/btcsuite/btcd/releases

btcwallet https://github.com/btcsuite/btcwallet/releases

## Notice

If you have already completed the above preparations, you can import the project with you IDE(my IDE is IntelliJ IDEA 2017.2.3). The IDE will help you to install some dependency packages, Please note the version number of the dependent package which is very important. 

## Getting Started:

run btcd:

    btcd -u rpcuser -P rpcpass (--testnet --mainnet)

create btcwallet:

    btcwallet -u rpcuser -P rpcpass --create

run bctwallet:

    btcwallet -u rpcuser -P rpcpass -d trace

run server.go and client.go

You can run the files in the IDE or in the command line.

If everything's working correctly, it'll say "listening on port 8082" or something like that and start downloading a lot of blocks. 
Afterwards, it'll just run. And then you can run the client.go,it will send a quest to the server and receive a response with a long signature at the end.

ps: We use a parallel strategy to simulate multiple users and test the time required to mix coins in different numbers of users. If you don't want user the Multi-threaded mode，you can comment the code in the client.go.

If you have any question, please send message to binge1638@163.com. Good luck.
