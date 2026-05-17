# Frissio Privacy Policy

**Last updated: May 2026**

The short version: Frissio collects nothing. There is no server. Your statements never leave your Mac.

---

## What Frissio collects

Nothing.

No usage analytics. No crash reports. No identifiers. No telemetry of any kind.

## Where your data lives

Everything — your transaction history, categories, rules, and account names — is stored in a single SQLite file on your Mac at:

```
~/Library/Application Support/com.frissio.desktop/frissio.db
```

You own that file. Back it up, move it, delete it. Frissio has no copy.

## Can Frissio connect to the internet?

No. The build ships without the `com.apple.security.network.client` entitlement. macOS itself enforces this — it is not a setting we control or could accidentally change in an update. You can verify it at any time: open Settings inside Frissio and look at the network request counter. It will always read 0.

For the technically curious: `codesign -d --entitlements - /Applications/Frissio.app` will show the entitlements list. The network client entitlement is not there.

## Third-party services

None. There are no third-party SDKs, analytics libraries, or cloud services bundled in the app.

## What happens if you email us

If you email support.frissio@gmail.com, we read your email and reply. We don't add you to a mailing list or share your address. That's it.

## Changes to this policy

If this ever changes — for example, if we add an optional cloud sync feature — we will update this document and surface the change prominently in the release notes before shipping. We will never collect data silently.

## Contact

support.frissio@gmail.com
