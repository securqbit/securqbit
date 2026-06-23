# FAQ

🔗 **Live:** [securqbit.com/#faq](https://securqbit.com/#faq)

> **Likely questions.**

---

### Does Securqbit really work behind strict firewalls?

Yes. The client probes the network, picks an obfuscated transport that survives inspection, and hops if the path is throttled. If one of our entry points is blocked in your country, the app rotates to one that isn't.

### Are you really no‑logs?

We keep no connection metadata, no DNS queries, no bandwidth accounting per‑user. Our servers run on volatile storage and reboot to a clean state. The only account data we keep is what's required to run your subscription. See the [No‑Log Policy](legal/no-log-policy.md).

### Which platforms do you support?

iOS and Android. Both clients are native — the iOS build uses the system Network Extension, the Android build integrates with Quick Settings, Tasker, and Android's VPN service. Desktop apps are on the roadmap.

### Will it drain my battery?

The tunnel is efficient on both iOS and Android. Our clients sleep aggressively when the screen is off and respect each OS's background power rules. Typical overhead is under 2% per day.

### What happens if the VPN disconnects?

Kill switch is on by default. If the tunnel drops for any reason — dead cell tower, captive portal, server hiccup — your device's network is held down until the tunnel reconnects. No accidental leaks.

---

**More:** [Features →](features.md) · [Security →](security.md) · [Pricing →](pricing.md) · [Support →](support.md)
