This project is for Catathon 2020. The aim is to modify the code in the "omnipay-btcpayserver" dir to become a standalone
packagist composer module.

TODO:

We're using the code in the "omnipay-btcpayserver" dir ([Canonical repo](https://github.com/dcentrica/omnipay-bitpay)) as our BTCPayServer Omnipay driver. Our aim is for this module-code to evolve into a supported, canonical packagist module for BTCPayServer-Omnipay integration. Its de-facto home on Github should be: https://github.com/dcentrica/omnipay-bitpay.

1. Configure the logic in the "omnipay-btcpayserver" dir with credentials/tokens etc for our BTCPayServer instance
2. Configure the included [silverstripe/silverstripe-omnipay](https://github.com/silverstripe/silverstripe-omnipay) module to use/consume "omnipay-btcpayserver" as its payment gateway/driver
3. Test according to the docs
4. If it fails and it's clear this older codebase isn't going to work - it will need to be modified by munging-in the latest [BTCPayServer PHP Client](https://github.com/btcpayserver/php-bitpay-client) or writing some glue code to make the two packages consume one another
