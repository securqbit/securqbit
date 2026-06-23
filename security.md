# Security

🔗 **Live:** [securqbit.com/#security](https://securqbit.com/#security)

> **Simple primitives. Public scrutiny. No secret sauce.**

The cryptography is the same stack your browser and SSH client rely on. What's novel is how we survive hostile networks without compromising any of it.

---

## Security architecture

| Layer | Detail |
|-------|--------|
| **Transport** | Obfuscated · adaptive · stealth fallback |
| **Encryption** | Industry‑standard AEAD |
| **Key exchange** | Forward‑secret · post‑quantum ready |
| **Integrity** | Authenticated at every packet |
| **Server disk** | Volatile only. Logs impossible. |
| **Jurisdiction** | Audit‑friendly, privacy‑respecting |

## Packet path (simplified)

```
Your phone  ──▶  Firewall  ──▶  Edge relay  ──▶  Core node  ──▶  Destination
 obfuscated     stealth        encrypted        direct
```

1. **Your phone → Firewall** — obfuscated transport; *looks like ordinary HTTPS*.
2. **Firewall → Edge relay** — stealth path; *rotates every ~90 seconds*.
3. **Edge relay → Core node** — encrypted; *no logs, volatile disk*.
4. **Core node → Destination** — direct; *exit pool*.

## Why this design

- **No secret sauce.** We use the same authenticated‑encryption primitives modern browsers and SSH clients trust. There's no proprietary crypto to get wrong — the security comes from public, scrutinized building blocks.
- **Survival under inspection.** The obfuscation and adaptive hopping happen *around* the crypto, not instead of it, so traffic survives deep packet inspection without weakening encryption.
- **Logs are architecturally impossible.** Servers run on volatile (RAM‑based) storage and reboot to a clean state — there's no persistent disk to retain user activity. See the [No‑Log Policy](legal/no-log-policy.md).
- **Forward secrecy + post‑quantum readiness.** Key exchange is forward‑secret (a compromised key can't decrypt past sessions) and built to adopt post‑quantum primitives.

## What a VPN does *not* do

A VPN protects the transport of your traffic; it does not make you anonymous in every context:

- Sites you log into can still identify you through your account credentials.
- Cookies, browser fingerprints, and third‑party trackers are outside a VPN's scope.
- Malware or a compromised device can expose activity regardless of VPN use.
- Local networks, ISPs, or operating systems may keep their own records.

## Reporting a vulnerability

Security or legal inquiries: **[security@securqbit.com](mailto:security@securqbit.com)**

---

**Next:** [Download & verify →](download.md) · [No‑Log Policy →](legal/no-log-policy.md)
