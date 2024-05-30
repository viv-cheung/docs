fr + fr-translated # Channels
fr + fr-translated A channel is a public space for your community to have conversations around a topic.
fr + fr-translated Creating a channel starts a new feed for your community. People can join, cast and find other interesting people. It sparks conversations that wouldn’t otherwise happen on the home feed.
fr + fr-translated :::warning Experimental Feature
fr + fr-translated Channels are being prototyped in Warpcast and not fully supported by the Farcaster protocol. They may be ported to the protocol in the future if the feature is deemed successful or they may be removed entirely.
fr + fr-translated :::
fr + fr-translated ## Hosting Channels
fr + fr-translated Anyone can create a channel host by paying a fee in Warpcast and choosing a channel name. The name must be under 16 characters and can only contain lowercase alphabets and numbers. A channel's creator is called a host and may invite other co-hosts to operate the channel. Hosts have special privileges like:
fr + fr-translated 1. Defining “channel norms" which everyone must agree to when joining.
fr + fr-translated 2. Pinning or hiding casts in a channel.
fr + fr-translated 3. Blocking other users from casting in their channel.
fr + fr-translated 4. Setting a channel picture, description and other metadata.
fr + fr-translated Channel metadata is not part of the protocol and stored in Warpcast while channels are in the experimental stage.
fr + fr-translated ## Casting in Channels
fr + fr-translated Anyone can post into a channel by using Warpcast and selecting the channel when creating the cast. Warpcast automatically sets the cast's `parentUrl` to `https://warpcast.com/~/channel/<name>`. A cast is considered "in a channel" if it's parentUrl is the channel URI or another cast which is "in a channel".
fr + fr-translated Channel casts are part of the protocol and stored on hubs. Using a replicator, you can fetch all casts in a channel by filtering the `parentUrl` field for the channel's FIP-2 URL.
fr + fr-translated ## Following Channels
fr + fr-translated Anyone can follow a channel just like a user. A user will see casts from a followed channel in their home feed when using Warpcast.
fr + fr-translated Channel follows are not part of the protocol and are stored in Warpcast while channels are in the experimental stage.
fr + fr-translated ## Cast Visibility
fr + fr-translated If a user casts in a channel, Warpcast will:
fr + fr-translated 1. Always send the casts to the home feeds of any user who follows the channel.
fr + fr-translated 2. Usually send the casts to the home feeds of any user who follows the author.
fr + fr-translated The determination for (2) is made based on the user's preferences, channel contents and other social graph data. This algorithm is still being fine tuned and will be documented once it is stable.
fr + fr-translated ## Usage Policy
fr + fr-translated Warpcast may remove your channel and will NOT refund your warps if:
fr + fr-translated 1. Your profile or channel impersonates someone.
fr + fr-translated 2. You squat a channel without using it.
fr + fr-translated 3. You violate Warpcast's terms and conditions or app store rules.
fr + fr-translated ## FAQ
fr + fr-translated **Why are channel hosts allowed to hide and ban? Isn’t this censorship?**
fr + fr-translated Channels are not free-for-all public spaces, they are owned and moderated by their creators. You are always free to start your own channel at any time with its own rules.
fr + fr-translated **Why is there a fee for creating channels?**
fr + fr-translated The fee discourages people from squatting short names and not using the channels.
fr + fr-translated **What's the benefit of creating a channel?**
fr + fr-translated Starting a channel also helps grow your audience:
fr + fr-translated 1. Warpcast will send your followers a notification about your channel.
fr + fr-translated 2. Your channel will be promoted to users who follow similar channels.
fr + fr-translated 3. Users who follow your channel will see channel casts in their home feed.
fr + fr-translated ## Resources
fr + fr-translated ### APIs
fr + fr-translated - [Warpcast Channel APIs](../../reference/warpcast/api.md) - fetch a list of all known channels