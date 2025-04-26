# Multicar: Multisynq plus Three.js

This is an example of combining Multisynq for multiplayer and Three.js for 3D rendering in a single-page game. Mostly as an example for AI vibe-coding.

The original car game this is based on was vibe-coded by [mrdoob](https://x.com/mrdoob/status/1904829276530016641). The version here does not change the gameplay at all, only makes it multiplayer.

We do so by using the [Multisynq client library](https://multisynq.io/docs/client) which accesses the *Multisynq DePIN* network via a [Multisynq API key](https://multisynq.io/coder).

In Multisynq, the multiplayer logic does not run on a server, but the "server logic" runs on identical VMs in each client. You can use almost any JavaScript language construct, for example for collision detection, without having to use special data structures and without explicitly synchronizing changes.

Multisynq keeps these Multisynq VMs in sync by providing a global decentralized network of "synchronizers." They ensure all VMs in a session process the exact same stream of events at the same time, so they all stay in sync.

Each session is end-to-end encrypted by a random session name and password. These are automatically added to the URL. Another player can join either by copy-pasting that URL, or by scanning the QR code in the top-right.

## How to run
To try this game, simply double-clicking the HTML file to open it in a web browser should work.

To deploy it, change the API key to your own (from multisynq.io/coder) and upload the HTML file to any web server (for example, GitHub Pages).

## How to use with AI

Give the HTML file to the AI as context, and tell it to build a multiplayer game based on this example.
