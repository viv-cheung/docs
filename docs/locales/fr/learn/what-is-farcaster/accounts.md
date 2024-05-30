fr + fr-translated # Accounts
fr + fr-translated A Farcaster account lets you set up a username, profile picture and publish short text messages known as casts. Any Ethereum address can register a Farcaster account by making an onchain transaction.
fr + fr-translated ## Creating an account
fr + fr-translated A Farcaster account is created by calling the IdGateway contract. It will assign a new Farcaster ID or fid to your Ethereum address.
fr + fr-translated You'll need to get a username, rent storage and add a key before you can use your account. These steps require many signatures and onchain transactions and can be tedious with a regular Ethereum wallet.
fr + fr-translated We recommend starting with [Warpcast](https://www.warpcast.com/), a special Farcaster wallet which will handle the entire flow for you. It also uses a separate Ethereum account to sign transactions, so you can keep your main Ethereum account secure.
fr + fr-translated ## Adding account keys
fr + fr-translated Accounts can issue keys which let apps write messages on their behalf. Users will typically issue a key to each Farcaster app they use.
fr + fr-translated Keys are managed by the KeyRegistry contract. To add a key, you'll need to submit the public key of an EdDSA key pair along with a requestor signature. The requestor can be the account itself or an app that wants to operate on its behalf.
fr + fr-translated ## Recovering an account
fr + fr-translated Users often set up separate wallets for their social apps and it's easy to lose access. Farcaster lets any account specify a recovery address which can be used to recover the account. It can be configured when creating the account or anytime after.
fr + fr-translated Users can set the recovery address to trusted services like Warpcast or they can manage it themselves using a regular Ethereum wallet.
fr + fr-translated ## Resources
fr + fr-translated ### Specifications
fr + fr-translated - [Contract Specifications](https://github.com/farcasterxyz/protocol/blob/main/docs/SPECIFICATION.md#1-smart-contracts) - The onchain contracts that manage Farcaster accounts, account keys and recovery addresses.
fr + fr-translated ### APIs
fr + fr-translated - [IdRegistry](../../reference/contracts/reference/id-registry) - Lookup account data onchain.
fr + fr-translated - [IdGateway](../../reference/contracts/reference/id-gateway) - Create accounts onchain.
fr + fr-translated - [KeyRegistry](../../reference/contracts/reference/key-registry) - Lookup account key data onchain.
fr + fr-translated - [KeyGateway](../../reference/contracts/reference/key-gateway) - Create account keys onchain.
fr + fr-translated - [Get Farcaster Ids](../../reference/hubble/httpapi/fids) - Fetch a list of all registered account fids from a hub.
fr + fr-translated - [Get account keys](../../reference/hubble/httpapi/onchain#onchainsignersbyfid) - Fetch the account keys (signers) for an account from a hub.
fr + fr-translated ### Tutorials
fr + fr-translated - [Create an account](../../developers/guides/accounts/create-account.md) - Create a new account on Farcaster.
fr + fr-translated - [Create an account key](../../developers/guides/accounts/create-account-key.md) - Create a new account key for your account.
fr + fr-translated - [Find account by username](../../developers/guides/accounts/find-by-name.md) - Find an account by its username.
fr + fr-translated - [Change custody address](../../developers/guides/accounts/change-custody.md) - Change the address that owns your account.
fr + fr-translated - [Change recovery address](../../developers/guides/accounts/change-recovery.md) - Change the address that recovers your account.
fr + fr-translated - [Find account key requestor](../../developers/guides/advanced/decode-key-metadata.md) - Find the app that the user granted an account key to.
fr + fr-translated - [Query signups from replicator](../../developers/guides/advanced/query-signups.md) - Query the number of signups from the replicator.