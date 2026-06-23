# How it works

🔗 **Live:** [securqbit.com/#how](https://securqbit.com/#how)

> **Three steps. No settings. No VPN glossary to learn.**

---

### Step 1 — Install from the App Store or Google Play

One tap. iOS 20+ or Android 10+. See [Download](download.md) for store links and the verifiable signed APK.

### Step 2 — Tap connect

The client probes your network, picks the path that works, and negotiates a tunnel. Under a second on most networks.

### Step 3 — That's it

The icon in your status bar stays green. We stay out of the way. The firewall stays confused.

---

## Under the hood

When you tap connect, the client:

1. **Probes the network** to find which paths are open and which are throttled or inspected.
2. **Picks an obfuscated transport** that survives deep packet inspection — to the network it looks like ordinary HTTPS.
3. **Negotiates a tunnel** with forward‑secret key exchange and authenticated encryption.
4. **Hops adaptively** if a path degrades, rotating entry points so a single block doesn't drop your connection.

If the tunnel ever drops, the default‑on [kill switch](features.md#kill-switch--split-tunnel) holds your device's network down until it reconnects — no accidental leaks.

For the full transport and cryptography breakdown, see [Security](security.md).

---

**Next:** [Security →](security.md) · [Download →](download.md)
