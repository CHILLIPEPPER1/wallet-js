# Trip Wallet SDK for JavaScript

## API

## Attributes
* privateKey
* publicKey
* address
* currency

## Methods
* generate([currency]): Wallet
* import(key [, type] [, currency]): Wallet
    * type: 'privateKey', 'keystore', 'mnemonicPhrase', 'readonly'
    * key: string
    * currency: string
* setProvider(host)
* getBalance(addressHexString): Promise
* getTokenBalance(addressHexString, contractAddress): Promise
* getTransaction(transactionHash): Promise
* sendTransaction(transactionObject): Promise
* _encodeAbi(methodName, paramsName[], paramsValue[]): string
* _signTx(transactionObject): string
