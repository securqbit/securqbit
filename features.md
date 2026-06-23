# Features

🔗 **Live:** [securqbit.com/#features](https://securqbit.com/#features)

> **Boring reliability. Quiet privacy. No drama.**

Six things we've built, and a lot of things we've deliberately left out.

---

## Bypasses any firewall

Obfuscated traffic with adaptive protocol hopping — looks like ordinary HTTPS to deep packet inspection. If one of our entry points is blocked in your country, the app rotates to one that isn't.

## Zero logs, by design

No connection logs, no DNS logs, no bandwidth logs. The only thing we can hand over is nothing. See the [No‑Log Policy](legal/no-log-policy.md) for the binding commitment.

## Fast, on weak networks

Tuned transports with smart congestion control. Holds up on 3G, congested Wi‑Fi, and hotel networks.

## Kill switch & split tunnel

If the tunnel drops, the network drops. The kill switch is **on by default**. Per‑app split tunneling routes only what you choose.

## Modern cryptography

Industry‑standard authenticated encryption — the same primitives modern browsers trust. Forward‑secret key exchange, post‑quantum ready, authenticated at every packet. More in [Security](security.md).

## iOS & Android, done properly

Native clients on both platforms — battery‑aware, system‑integrated, and built by people who actually use their phones. The iOS build uses the system Network Extension; the Android build integrates with Quick Settings, Tasker, and Android's VPN service. Desktop apps are on the roadmap.

---

## Summary table

| Feature | What it means |
|---------|---------------|
| Firewall bypass | Obfuscated + adaptive protocol hopping; looks like HTTPS to DPI |
| Zero logs | No connection, DNS, or per‑user bandwidth logs |
| Fast on weak networks | Tuned transports + smart congestion control |
| Kill switch & split tunnel | Default‑on kill switch; per‑app routing |
| Modern cryptography | AEAD, forward‑secret, post‑quantum ready |
| Native clients | iOS Network Extension; Android Quick Settings/Tasker/VPN service |

---

**Next:** [How it works →](how-it-works.md) · [Security →](security.md) · [Download →](download.md)
