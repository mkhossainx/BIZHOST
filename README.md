# 💀 BIZHOST v2.0 — PHP Hosting Terminal

> A powerful, professional localhost hosting tool for Termux  
> Designed for mobile developers, testers, and cyber enthusiasts.

BIZHOST turns your Android device into a PHP hosting environment with public internet access — all from a sleek cyber terminal interface.

---

## ⚡ What's New in v2.0

- ✅ **Live status panel** — See SERVER and TUNNEL status right in the menu
- ✅ **Background tunnel** — Tunnel runs in background, you can return to menu
- ✅ **Separate Stop Tunnel option** — Kill tunnel without stopping server
- ✅ **Custom port support** — Change from default 8080 anytime
- ✅ **Colored server logs** — View live logs with color-coded status codes
- ✅ **System Info panel** — PHP version, cloudflared version, disk usage
- ✅ **Smarter install** — Pre-flight internet/Termux checks, fallback cloudflared download
- ✅ **Better index.php** — Clean dark-themed default landing page
- ✅ **Bug fixes** — Stop server now uses stored PID (won't kill unrelated PHP), config uses key=value format

---

## 📦 Requirements

- Android device
- Termux (latest version from F-Droid recommended)
- Internet connection (for installation & public link)
- Storage permission enabled

---

## 🚀 Installation

Open Termux and run:

```bash
apt update && apt install git -y
git clone https://github.com/mkhossainx/BIZHOST.git
cd BIZHOST
chmod +x install bizhost
./install
```

---

## ▶️ Usage

```bash
bizhost
```

---

## 🧭 Menu Options

| Option | Action |
|--------|--------|
| `[1]` | Start PHP server (with auto-restart watchdog) |
| `[2]` | Create public Cloudflare tunnel (runs in background) |
| `[3]` | Stop tunnel only |
| `[4]` | Stop server (and tunnel) |
| `[5]` | Open site folder in shell |
| `[6]` | Set site directory |
| `[7]` | Set custom port |
| `[8]` | View server logs (color-coded) |
| `[9]` | System info |
| `[U]` | Update BIZHOST |
| `[X]` | Exit |

---

## 📁 Website Location

```
/storage/emulated/0/BIZHOST/
```

Default entry point: `index.php`

---

## 🔧 Config

Config is stored at `$PREFIX/tmp/bizhost.conf` as key=value pairs:

```
SITE="/storage/emulated/0/BIZHOST"
PORT=8080
```

---

## ⚙️ How It Works

- PHP built-in development server (port configurable, default 8080)
- Watchdog subprocess auto-restarts PHP if it crashes
- Cloudflare Quick Tunnel for public access (background process)
- Config persisted to Termux tmp

---

## 🛡️ Security Notes

- Public links are temporary and expire
- Do not host sensitive data publicly
- Use responsibly

---

## 💻 Supported Platforms

- ✅ Android (Termux)
- ❌ Not designed for Windows / iOS

---

## ⚠️ Disclaimer

For educational and development purposes only.  
The author is not responsible for misuse.

---

## 👨‍💻 Author

**@bizft — BIZ FACTORY**  
Cyber Tools • Mobile Hosting • Terminal Utilities

---

## 💀 BIZHOST — Power in Your Pocket
