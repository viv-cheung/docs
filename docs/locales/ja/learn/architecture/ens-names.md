ja + ja-translated # ENS Names

ja + ja-translated Farcaster uses ENS names as human readable identifiers for accounts. Two kinds of ENS names are supported:

ja + ja-translated - **Offchain ENS Names**: free and controlled by farcaster. (e.g. @alice)
- **Onchain ENS Names**: costs money and controlled by your wallet. (e.g. @alice.eth)

ja + ja-translated ENS names can only be used on Farcaster if they are <= 16 characters and contain only lowercase letters, numbers and hyphens.

ja + ja-translated ![Usernames](/assets/usernames.png)

ja + ja-translated ## Onchain ENS Names

ja + ja-translated Users can use onchain ENS names like `@alice.eth` on Farcaster.

ja + ja-translated Onchain ENS names are issued by ENS, end in .eth and must be registered on the Ethereum L1 blockchain. Anyone can register an ENS name by using the [ENS app](https://app.ens.domains/).

ja + ja-translated Users must pay a fee to register an onchain ENS name, but once registered it is controlled by the user and cannot be revoked.

ja + ja-translated ## Offchain ENS Names (Fnames)

ja + ja-translated Users can use offchain ENS names like `@alice` on Farcaster.

ja + ja-translated Offchain ENS names, also called Farcaster Names or fnames, are compliant with ENS but registered offchain. Fnames are free but are subject to a usage policy to prevent squatting and impersonation. They are also subject to the following requirements:

ja + ja-translated 1. An account can only have one fname at a time.
2. An account can change its fname once every 28 days.

ja + ja-translated ### Usage Policy

ja + ja-translated Registering an fname is free but subject to the following policy:

ja + ja-translated 1. Names connected to public figures or entities may be reclaimed (e.g. @google).
2. Names that haven't been used for 60+ days may be reclaimed.
3. Names that are registered for the sole purpose of resale may be reclaimed.

ja + ja-translated Decisions are made by the Farcaster team and often require human judgement. Users who want a name that is fully under their control should use an onchain ENS name.

ja + ja-translated ### Registry

ja + ja-translated Fnames are issued as offchain names under the subdomain `fcast.id`.

ja + ja-translated Bob can register the offchain ENS name `bob.fcast.id` and use it on any Farcaster app with the shorthand `@bob`. The name can be registered by making a signed request to the Fname Registry server. See the FName API reference for more details on how to query and create fnames.

ja + ja-translated To learn more about how fnames work, see [ENSIP-16](https://docs.ens.domains/ens-improvement-proposals/ensip-16-offchain-metadata)
and [ERC-3668](https://eips.ethereum.org/EIPS/eip-3668).
