# Security Policy

## Supported Versions

| Version | Supported |
|---------|-----------|
| v6.0 (Portalv7) | ✅ Active |
| v5.x and earlier | ❌ Not supported |

## Reporting a Vulnerability

Auracelle Charlie is a client-side-only HTML simulation. It does not have a server,
does not store data externally, and does not transmit participant data to any third party.

If you discover a security vulnerability — for example, an XSS vulnerability in
the simulation that could be exploited if the file is hosted on a shared server —
please report it **privately** to:

**grace-alice.evans@bathspa.ac.uk**

Subject: `[SECURITY] Auracelle Charlie — [Brief description]`

Please do not open a public GitHub Issue for security vulnerabilities.

## Data handling

- Participant session data is stored in browser `localStorage` via safe wrappers
  that silently fail in Blob URL context
- No data is sent to any external server by the simulation itself
- The Anthropic API (Tab ⑩ Agentic AI) is only called if the participant
  explicitly enters their own API key — no key is bundled with the simulation
- API keys entered in Tab ⑩ are stored in `sessionStorage` only and cleared
  when the browser tab is closed

## Known limitations

- The simulation is a single HTML file opened locally or via GitHub Pages
- Local file:// protocol restricts some browser APIs (localStorage, clipboard)
  which is handled by the safeLocal wrapper functions
- The Blob URL approach used to launch Charlie from the portal is intentional and
  does not represent a security vulnerability
