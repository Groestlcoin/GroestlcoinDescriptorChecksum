# GroestlcoinDescriptorChecksum

* Computes the descriptor checksum for public as well as private keys, unlike the groestlcoin RPC getdescriptorinfo (groestlcoin-core v2.18.2)
* Descriptors containing private keys can be used to derive hardened child keys with the RPC deriveaddresses (e.g. the groestlcoin-core keypath m/0'/0'/i')
* For details on the format of a descriptor, see [Support for Output Descriptors in Groestlcoin Core](https://github.com/Groestlcoin/groestlcoin/blob/v2.18.2/doc/descriptors.md)
* Standalone version of the code found [here](https://github.com/Groestlcoin/groestlcoin/blob/v2.18.2/src/script/descriptor.cpp)

## Installation

Requires:

* GNU Make v4.1
* g++ v5.4.0

To compile:

* Type `make all`

## Usage Example

* Usage: groestlcoin_descriptor_checksum "descriptor"
* The example below was generated on a `regtest` network:
```
$ ./groestlcoin_descriptor_checksum "raw(76a914068ed53e0759142ad97b928fc4b246f78d7b41f288ac)"
$ raw(76a914068ed53e0759142ad97b928fc4b246f78d7b41f288ac)#sqwyljrc
```
