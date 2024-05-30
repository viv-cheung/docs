fr + fr-translated # ENS Names
fr + fr-translated Farcaster uses ENS names as human readable identifiers for accounts. Two kinds of ENS names are supported:
fr + fr-translated - **Offchain ENS Names**: free and controlled by farcaster. (e.g. @alice)
fr + fr-translated - **Onchain ENS Names**: costs money and controlled by your wallet. (e.g. @alice.eth)
fr + fr-translated ENS names can only be used on Farcaster if they are <= 16 characters and contain only lowercase letters, numbers and hyphens.
fr + fr-translated ![Usernames](/assets/usernames.png)
fr + fr-translated ## Onchain ENS Names
fr + fr-translated Users can use onchain ENS names like `@alice.eth` on Farcaster.
fr + fr-translated Onchain ENS names are issued by ENS, end in .eth and must be registered on the Ethereum L1 blockchain. Anyone can register an ENS name by using the [ENS app](https://app.ens.domains/).
fr + fr-translated Users must pay a fee to register an onchain ENS name, but once registered it is controlled by the user and cannot be revoked.
fr + fr-translated ## Offchain ENS Names (Fnames)
fr + fr-translated Users can use offchain ENS names like `@alice` on Farcaster.
fr + fr-translated Offchain ENS names, also called Farcaster Names or fnames, are compliant with ENS but registered offchain. Fnames are free but are subject to a usage policy to prevent squatting and impersonation. They are also subject to the following requirements:
fr + fr-translated 1. An account can only have one fname at a time.
fr + fr-translated 2. An account can change its fname once every 28 days.
fr + fr-translated ### Usage Policy
fr + fr-translated Registering an fname is free but subject to the following policy:
fr + fr-translated 1. Names connected to public figures or entities may be reclaimed (e.g. @google).
fr + fr-translated 2. Names that haven't been used for 60+ days may be reclaimed.
fr + fr-translated 3. Names that are registered for the sole purpose of resale may be reclaimed.
fr + fr-translated Decisions are made by the Farcaster team and often require human judgement. Users who want a name that is fully under their control should use an onchain ENS name.
fr + fr-translated ### Registry
fr + fr-translated Fnames are issued as offchain names under the subdomain `fcast.id`.
fr + fr-translated Bob can register the offchain ENS name `bob.fcast.id` and use it on any Farcaster app with the shorthand `@bob`. The name can be registered by making a signed request to the Fname Registry server. See the [FName API reference](/reference/fname/api) for more details on how to query and create fnames.
fr + fr-translated To learn more about how fnames work, see [ENSIP-16](https://docs.ens.domains/ens-improvement-proposals/ensip-16-offchain-metadata)
fr + fr-translated and [ERC-3668](https://eips.ethereum.org/EIPS/eip-3668).