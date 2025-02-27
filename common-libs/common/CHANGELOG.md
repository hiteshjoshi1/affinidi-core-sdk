# 2.0.0-beta.7 (2021-08-30)
* `Affinity` constructor now requires `IPlatformCryptographyTools` parameter
* Implemented support for BBS and RSA (key generation, signing, validation), if relevant `IPlatformCryptographyTools` is provided
* Improved types
* New `generateSeed` method is exported
* Document loader now caches schemas loaded frow w3.org and w3id.org
# 2.0.0-beta.6 (2021-08-23)
* export `LocalKeyService`
* Add `asyncSign` to `KeyVault` to simplify usage of the library in async contexts
* export `LocalKeyService` implements `asyncSign`
# 2.0.0-beta.5 (2021-08-20)
* `ElemDidDocument` abstracted to use a KeyVault to provide the relevant keys
# 2.0.0-beta.4 (2021-07-23)
* Fixed initializing `externalKeys` in `KeysService`
# 2.0.0-beta.3 (2021-07-19)
* Internal changes
# 2.0.0-beta.1 (2021-06-29)
* Improved type declarations
* Breaking changes
  * `KeysService.getSigningKey` and `getKey` made private. Use one of the following alternatives instead:
    * `getPublicKey`
    * `getPrivateKey`
    * `getPublicAndPrivateKeys`
    * `getAnchorTransactionPublicKey`
    * `getAnchorTransactionPrivateKey`
    * `getAnchorTransactionPublicAndPrivateKeys`
# 1.9.0 (2020-06-16)
* Declared input and output types on `KeysService` methods
* Implemented `KeysService.getOwnPublicKey` and `KeysService.getOwnPrivateKey`
# 1.8.0 (2020-06-04)
* Reorganized dependencies
# 1.6.0 (2020-02-16)
* Performance improvement. Add revocable credential context url to [local context](./src/_baseDocumentLoader/localContexts.ts) .
