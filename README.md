# Multicar: Multisynq plus Three.js

This is an example of combining Multisynq for multiplayer and Three.js for 3D rendering in a single-page game. Mostly as an example for AI vibe-coding.

The original car game this is based on was vibe-coded by [mrdoob](https://x.com/mrdoob/status/1904829276530016641). The version here does not change the gameplay at all, only makes it multiplayer.

We do so by using the [Croquet 2.0 library](https://multisynq.io/docs/croquet) which accesses the *Multisynq DePIN* network via an [API key](https://multisynq.io/coder).

In Croquet, the multiplayer logic does not run on a server, but the "server logic" runs on identical VMs in each client. You can use almost any JavaScript language construct, for example for collision detection, without having to use special data structures and without explicitly synchronizing changes.

Multisynq keeps these Croquet VMs in sync by providing a global decentralized network of "synchronizers." They ensure all VMs in a session process the exact same stream of events at the same time, so they all stay in sync.

Each session is end-to-end encrypted by a random session name and password. These are automatically added to the URL. Another player can join either by copy-pasting that URL, or by scanning the QR code in the top-right.

Croquet 2.0 is open-source, you can find it on [npm](https://www.npmjs.com/package/@croquet/croquet) and [GitHub](https://github.com/croquet/croquet). Note that only [version 2](https://www.npmjs.com/package/@croquet/croquet?activeTab=versions) is compatible with Multisynq.
