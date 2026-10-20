# Changelog

## 1.5 — 2026-10-21

- History marks IPs that came through a VPN with a "VPN" tag, also exported as a VPN column in CSV.
- Identifies the VPN in use: its name (e.g. NordVPN, ProtonVPN) and Tailscale exit nodes, with the exit node's name. Both can be turned off in Settings → Display.

## 1.4 — 2026-10-21

- With a VPN, the menu bar now shows only the current public (VPN) IP. Choose "ISP IP → VPN IP" in Settings → Display to show both.
- Fixed typing a check interval (e.g. "10" turned into "50").
- Fixed the ISP IP shrinking and growing in the overview while a VPN is on.
- Fixed the "VPN blocks all traffic outside the tunnel" note appearing and disappearing while a VPN is on.

## 1.3 — 2026-10-21

- Three more IP reputation services that need no API key: fFraud, ip-api.com and StopForumSpam (Settings → Reputation). proxycheck.io remains the default.

## 1.2.1 — 2026-10-21

- Fixed VPNs that send all traffic through the tunnel being reported as "split tunnel". When such a VPN hides the ISP IP, the last ISP IP seen before the VPN is shown instead.

## 1.2 — 2026-10-21

- Set a maximum number of history entries (50, 100, 200, 500, 1,000 or unlimited) in Settings → History, alongside auto-delete. Oldest entries are removed first.

## 1.1 — 2026-10-21

First public release.

- Public IP and short ISP name in the menu bar (`VNPT · 203.0.113.45`), with short names for providers worldwide.
- VPN aware: shows both the VPN IP and the original ISP IP.
- Re-checks right away when the network drops and comes back or the Mac wakes; otherwise every 3 minutes (adjustable).
- IP history recorded only when the IP changes, with automatic cleanup (6 hours to 1 month) and CSV export.
- Popup when the IP changes (1–5 s, top left / center / right), noting when a returning IP was last used.
- IP reputation score from proxycheck.io, AbuseIPDB or IPQualityScore.
- Local IPv4 / IPv6 per network interface.
- One-click updates: downloads, verifies (SHA-256), installs and reopens.
- English and Vietnamese, light and dark mode, open at login.
