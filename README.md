# Bitcore-Innova

[![NPM Package](https://img.shields.io/npm/v/bitcore-innova.svg?style=flat-square)](https://www.npmjs.org/package/bitcore-innova)
[![Build Status](https://img.shields.io/travis/innovacoin/bitcore-innova.svg?branch=master&style=flat-square)](https://travis-ci.org/innovacoin/bitcore-innova)

Infrastructure to build Innova and blockchain-based applications for the next generation of financial technology.

**Note:** If you're looking for the Bitcore-Innova Library please see: https://github.com/innovacoin/bitcore-lib-innova

## Getting Started

Before you begin you'll need to have Node.js v4+ installed. There are several options for installation. One method is to use [nvm](https://github.com/creationix/nvm) to easily switch between different versions, or download directly from [Node.js](https://nodejs.org/).

```bash
npm install -g bitcore-innova
```

Spin up a full node and join the network:

```bash
npm install -g bitcore-innova
bitcored
```

You can then view the Insight block explorer at the default location: `http://localhost:3001/insight`, and your configuration file will be found in your home directory at `~/.bitcore`.

Create a transaction:
```js
var bitcore = require('bitcore-innova');
var transaction = new bitcore.Transaction();
var transaction.from(unspent).to(address, amount);
transaction.sign(privateKey);
```

## Applications

- [Node-Innova](https://github.com/innovacoin/bitcore-node-innova) - A full node with extended capabilities using Innova Core
- [Insight API-Innova](https://github.com/innovacoin/insight-api-innova) - A blockchain explorer HTTP API
- [Insight UI-Innova](https://github.com/innovacoin/insight-ui-innova) - A blockchain explorer web user interface
- [Wallet Service](https://github.com/innovacoin/bitcore-wallet-service-innova) - A multisig HD service for wallets
- [Wallet Client](https://github.com/innovacoin/bitcore-wallet-client-innova) - A client for the wallet service
- CLI Wallet - A command-line based wallet client
- Angular Wallet Client - An Angular based wallet client
- Copay - An easy-to-use, multiplatform, multisignature, secure Innova wallet

## Libraries

- [Lib-Innova](https://github.com/innovacoin/bitcore-lib-innova) - All of the core Innova primatives including transactions, private key management and others
- Payment Protocol - A protocol for communication between a merchant and customer
- [P2P-Innova](https://github.com/innovacoin/bitcore-p2p-innova) - The peer-to-peer networking protocol
- [Mnemonic-Innova](https://github.com/innovacoin/bitcore-mnemonic-innova) - Implements mnemonic code for generating deterministic keys
- Channel - Micropayment channels for rapidly adjusting Innova transactions
- [Message-Innova](https://github.com/innovacoin/bitcore-message-innova) - Innova message verification and signing
- [ECIES-Innova](https://github.com/innovacoin/bitcore-ecies-innova) - Uses ECIES symmetric key negotiation from public keys to encrypt arbitrarily long data streams.

## Documentation

The complete docs are hosted here: [bitcore documentation](http://bitcore.io/guide/). There's also a [bitcore API reference](http://bitcore.io/api/) available generated from the JSDocs of the project, where you'll find low-level details on each bitcore utility.

- [Read the Developer Guide](http://bitcore.io/guide/)
- [Read the API Reference](http://bitcore.io/api/)

To get community assistance and ask for help with implementation questions, please use our [community forums](http://bitpaylabs.com/c/bitcore).

## Security

We're using Bitcore in production, as are [many others](http://bitcore.io#projects), but please use common sense when doing anything related to finances! We take no responsibility for your implementation decisions.

If you find a security issue, please email security@bitpay.com.

## Contributing

Please send pull requests for bug fixes, code optimization, and ideas for improvement. For more information on how to contribute, please refer to our [CONTRIBUTING](https://github.com/innovacoin/bitcore-innova/blob/master/CONTRIBUTING.md) file.

This will generate files named `bitcore.js` and `bitcore.min.js`.

## License

Released under the MIT license, under the same terms as DashCore itself. See [LICENSE](LICENSE) for more info.
