# privacy-policy
# PAASMAN Advanced — Privacy Policy

**Effective date:** _fill in on publish_

PAASMAN Advanced is a local-first password vault. This page explains exactly
what the extension touches and where it goes.

## What we do NOT collect
- No telemetry, analytics, or crash reporting
- No account, email, or user ID
- No browsing history
- No vault content — ever

## What the extension accesses

| Scope | Why | Leaves device? |
|---|---|---|
| `storage` | Encrypted vault | No |
| `alarms` | Auto-lock timer | No |
| `clipboardWrite` | Copy user-selected values | To clipboard only (auto-cleared 30s) |
| `activeTab`, `scripting` | Detect password/card fields for autofill | No |
| `offscreen` | Clipboard auto-clear | No |
| `host <all_urls>` | Detect fillable fields on any site | No page content is read or transmitted |
| `api.lemonsqueezy.com` | License verification (once per 30 days) | Only your license key |
| `api.pwnedpasswords.com` | Breach check (opt-in, on demand) | Only a 5-character SHA-1 hash prefix; HIBP cannot reverse it |

## Where your vault lives
`chrome.storage.local`, encrypted with AES-256-GCM using a PBKDF2-SHA256
(600,000 iterations) key derived from your master password. The key is held
in memory in the service worker and never persisted to disk. Auto-locks on
your chosen interval, on browser close, and on panic-lock (`Ctrl+Shift+L`).

## Payment
Purchases are handled by **Lemon Squeezy**, the merchant of record. We never
see or store your card. Their privacy policy applies to that transaction.
After purchase, only the **license key** is stored locally — never payment info.

## Third-party services
- Lemon Squeezy: `https://www.lemonsqueezy.com/privacy`
- Have I Been Pwned: `https://haveibeenpwned.com/Privacy`

## Your rights
We hold no data about you. Delete the extension to delete your vault.
Export backups let you move your data to any tool that can decrypt the file
(you can even do it manually — it's just AES-GCM).

## Contact
If you have any questions, concerns, or feedback regarding this Privacy Policy or the security of your data, please contact us at:
• Email: sohailkhn18@gmail.com or contact (+91 8080192024)
• Developer/Company Name: Sohel Sarwar Khan
