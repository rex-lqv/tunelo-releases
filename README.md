# ⚡ Tunelo

**The missing GUI for SSH tunnels on macOS.**
Stop copy-pasting terminal commands. Manage all your tunnels in one place.

<p align="center">
  <img width="300" height="300" alt="Screenshot 2026-03-11 at 4 44 31 a m" src="https://github.com/user-attachments/assets/9f1cc5c6-3a7a-4610-b3c5-83516f6b589b" />
</p>

---


## Why Tunelo?

If you've ever found yourself running this every morning:

```bash
gcloud compute ssh my-vm --project=my-project -- -L 5432:localhost:5432 -N
```

Tunelo is for you. Save it once, connect with one click.

---

## Features

- ✅ **Free to start** — up to 3 tunnels, no account needed
- ✅ **Pro plan** — unlimited tunnels for $2.99 one-time
- ✅ **One-click connect/disconnect** — no more terminal copy-paste
- ✅ **Full PTY support** — handles password, passphrase prompts natively
- ✅ **Real-time output** — see exactly what's happening
- ✅ **Works with any SSH command** — GCP, AWS, DigitalOcean, plain SSH
- ✅ **macOS native** — dark mode, lives in your dock

---

## Download

👉 **[Download latest version](https://github.com/rex-lqv/tunelo-releases/releases/latest)**

> macOS 12+ required. Apple Silicon & Intel supported.

**First time install:**
```
Right click → Open → Open Anyway
```
*(Required because app is not yet notarized)*

---

## Quick Start

1. Download and install Tunelo
2. Click **"Add Your First Tunnel"**
3. Give it a name (e.g. `Production DB`)
4. Paste your SSH command:
   ```
   gcloud compute ssh my-vm --project=my-project -- -L 5432:localhost:5432 -N
   ```
5. Click **Save** → **Connect**

That's it. 🟢

---

## Examples

**GCP — forward PostgreSQL**
```
gcloud compute ssh my-vm --project=my-project --zone=asia-southeast1-a -- -L 5432:localhost:5432 -N
```

**AWS — forward RDS**
```
ssh -i ~/.ssh/key.pem -L 5432:rds-endpoint.amazonaws.com:5432 ec2-user@bastion-ip -N
```

**Plain SSH**
```
ssh -L 8080:localhost:8080 user@your-server.com -N
```

---

## Pricing

| Plan | Price | Tunnels |
|------|-------|---------|
| Free | $0 | Up to 3 |
| Pro  | $2.99 one-time | Unlimited |

👉 **[Get Pro](https://tunelo.lemonsqueezy.com/checkout/buy/04587353-2f20-479f-9cc0-6adcac9fee92)**

---

## Roadmap

- [ ] Structured form UI (GCP, AWS, Azure — no command knowledge needed)
- [ ] Auto-reconnect on disconnect
- [ ] Import/export config
- [ ] Menu bar mode

---

## Feedback & Issues

Found a bug? Have a feature request?
👉 [Open an issue](https://github.com/rex-lqv/tunelo-releases/issues)

---

*Built by a developer, for developers. Made in Vietnam 🇻🇳*
