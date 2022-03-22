# Arcadrex
Arcadrex is a method of displaying an Ethereum address as two roughly equal lines of text, each line an arc that intersects with the other, such that a 6-digit prefix of the address string and a 6-digit suffix of the address string appear adjacent to one another.

An Ethereum address represents an externally owned account (EOA) or contract that can receive (destination address) or send (source address) transactions on the blockchain. More specifically, it is the rightmost 160 bits of a Keccak hash of an elliptic curve digital signature algorithm (ECDSA) public key.

_Source: https://ethereum.org/en/glossary/_
  
_Externally Owned Address_ refers to an account with a public and private key pair that holds your funds.

An Ethereum address is a 42-character hexadecimal address derived from the last 20 bytes of the public key controlling the account with 0x appended in front. e.g., 0x71C7656EC7ab88b098defB751B7401B5f6d8976F.

The Ethereum address is the "public" address that you would need to receive funds from another party. To access funds in the address, you must have its private key. Kindly exercise duty of care when handling your private key as they can be used to access all the funds in an address.

A wallet is an interface that you may use to manage your Ethereum account as well as its public and private key pair. To get an Ethereum address/account to send and receive funds, kindly visit Etherscan Directory for a list of available wallets.

_Contract address_ refers to the address hosting a collection of code on the Ethereum blockchain that executes functions. These functions of a contract address are executed when a transaction with associated input data (contract interaction) is made to it.

The contract address is usually created when a contract is deployed to the Ethereum Blockchain.

Both Externally Owned and Contract Addresses share the same format of having 42 hexadecimal characters.

Etherscan differentiates between the two by displaying the Contract Creation field for Contract Addresses.

_Source: https://info.etherscan.com/what-is-an-ethereum-address/_

The Ethereum Name Service (ENS) is a distributed, open, and extensible naming system based on the Ethereum blockchain. ENS’s job is to map human-readable names like ‘alice.eth’ to machine-readable identifiers such as Ethereum addresses, other cryptocurrency addresses, content hashes, and metadata. ENS also supports ‘reverse resolution’, making it possible to associate metadata such as canonical names or interface descriptions with Ethereum addresses.

_Source: https://docs.ens.domains/_

While ENS vastly improves upon the UX of 42-character hexadecimal address strings when using Ethereum wallets to interact with Ethereum mainnet and supported Layer 2 (L2) networks, we still often encounter hex addresses and need a practical way of displaying them and comparing one to another in a manner that places minimal demand on attention and cognition.

Wallets and dapps often display hex addresses as a prefix of the string, followed by an ellipsis, followed by a suffix of the string, such that only the first and last 4-6 characters of the hex address are shown. This abbreviates the 42-character string to an 8-12 character string that most humans can easily process at a glance. The obvious tradeoff is that extra inputs are needed from the user to view the 42-character string in its entirety.

Arcadrex proposes to avoid this tradeoff by displaying an Ethereum address as two roughly equal lines of text, each line an arc that intersects with the other, such that a 6-digit prefix of the address string and a 6-digit suffix of the address string appear adjacent to one another. The 42-character hex address is split into two 21-character strings whose intersecting arcs create the impression of a third arc comprising 12 characters: the 6-character prefix and the 6-character suffix of the original 42-character string.
