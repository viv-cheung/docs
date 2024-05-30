fr + fr-translated # Usernames
fr + fr-translated A Farcaster account needs a username so it can be found and mentioned by other users. Farcaster uses the [Ethereum Name Service](https://ens.domains/) to manage usernames.
fr + fr-translated ENS usernames are owned by Ethereum addresses, just like Farcaster accounts. The difference is that an address can own multiple ENS names, so the Farcaster account must specify the name it wishes to use. Names must be less than 17 characters with only lowercase alphabets, numbers or hyphens to prevent homoglyph attacks.
fr + fr-translated ## Changing usernames
fr + fr-translated A Farcaster account can change between different usernames at any time. Changing names does not affect your history or your followers.
fr + fr-translated It's safe to change your name a few times a year. But changing your name more often may cause users or apps to lose trust in your account. If you want to change a public indicator, consider changing your display name instead.
fr + fr-translated ## Offchain vs Onchain Names
fr + fr-translated An account can choose between two kinds of usernames:
fr + fr-translated - **Offchain ENS Names**: free and controlled by farcaster. (e.g. @alice)
fr + fr-translated - **Onchain ENS Names**: costs money and controlled by your wallet. (e.g. @alice.eth)
fr + fr-translated Choose an offchain ENS name if you want to get started quickly and don't have an onchain ENS name. An account can always upgrade to an onchain name later. It's recommended to use an app like Warpcast to set this up for you.
fr + fr-translated ![Usernames](/assets/usernames.png)
fr + fr-translated ### Offchain ENS Names
fr + fr-translated - Offchain ENS names, also called fnames, are free and issued by Farcaster.
fr + fr-translated - Any Ethereum account can get one unique fname by calling the [Fname Registry](/learn/architecture/ens-names).
fr + fr-translated - Fnames are free but they can be revoked by Farcaster at any time.
fr + fr-translated ### Onchain ENS fnames
fr + fr-translated - Onchain ENS names, also called .eth names, are onchain and issued by ENS.
fr + fr-translated - Any Ethereum account can get an ENS by calling the [ENS Registry](https://docs.ens.domains/dapp-developer-guide/the-ens-registry).
fr + fr-translated - Names are not free but they cannot be revoked by Farcaster.
fr + fr-translated ## Resources
fr + fr-translated ### Specifications
fr + fr-translated - [Farcaster Name](https://github.com/farcasterxyz/protocol/blob/main/docs/SPECIFICATION.md#5-fname-specifications) - An ENSIP-10 offchain ENS name usable within Farcaster.
fr + fr-translated - [UserData: Username](https://github.com/farcasterxyz/protocol/blob/main/docs/SPECIFICATION.md#23-user-data) - Sets a valid Username Proof as the current username.
fr + fr-translated - [Username Proof](https://github.com/farcasterxyz/protocol/blob/main/docs/SPECIFICATION.md#17-username-proof) - Proves ownership of an onchain or offchain username.
fr + fr-translated - [Verifications](https://github.com/farcasterxyz/protocol/blob/main/docs/SPECIFICATION.md#25-verifications) - Proves ownership of an address, required for onchain Username Proofs.
fr + fr-translated ### APIs
fr + fr-translated - [UserData API](../../reference/hubble/httpapi/userdata) - Fetch the UserData for a user's current username.
fr + fr-translated - [Username Proofs API](../../reference/hubble/httpapi/usernameproof) - Fetch a user's Username Proofs from a hub.
fr + fr-translated - [Verification Proofs API](../../reference/hubble/httpapi/verification) - Fetch a user's Verifications from a hub.
fr + fr-translated - [Fname Registry API](../../reference/fname/api.md) - Register and track fname ownership programatically.
fr + fr-translated ### Tutorials
fr + fr-translated - [Get UserData](../../developers/guides/querying/fetch-profile.md) - Get UserData messages from an account.
fr + fr-translated - [Create UserData](../../developers/guides/writing/messages#user-data) - Create a UserData message to select a valid username.
fr + fr-translated - [Verify an Address](../../developers/guides/writing/verify-address.md) - Verify ownership of an Ethereum account.
fr + fr-translated - [Find account by username](../../developers/guides/accounts/find-by-name.md) - Find an account by its username.
fr + fr-translated - [Change farcaster name](../../developers/guides/accounts/change-fname.md) - Change a farcaster username.