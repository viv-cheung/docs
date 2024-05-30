fr + fr-translated # Architecture
fr + fr-translated Farcaster has a hybrid architecture that stores identity onchain and data offchain.
fr + fr-translated ![Architecture](/assets/architecture.png)
fr + fr-translated ## Onchain
fr + fr-translated Farcaster's onchain systems are implemented as [contracts on OP Mainnet](./contracts.md). Actions are performed onchain only when security and consistency are critical. Use of onchain actions is kept at a minimum to reduce costs and improve performance.
fr + fr-translated Only a handful of actions are performed onchain, including:
fr + fr-translated - Creating an [account](../what-is-farcaster/accounts.md).
fr + fr-translated - Paying rent to [store data](../what-is-farcaster/messages.md#storage).
fr + fr-translated - Adding account keys for [connected apps](../what-is-farcaster/apps.md#connected-apps).
fr + fr-translated ## Offchain
fr + fr-translated Farcaster's offchain system is a peer-to-peer network of servers called [Hubs](./hubs.md) which store user data. The majority of user actions are performed offchain. These include:
fr + fr-translated - Posting a new public message.
fr + fr-translated - Following another user.
fr + fr-translated - Reacting to a post.
fr + fr-translated - Updating your profile picture.
fr + fr-translated Actions are performed offchain when performance and cost are critical. Use of offchain actions is typically preferred when consistency isn't a strict requirement. Offchain systems achieve security by relying on signatures from onchain systems.