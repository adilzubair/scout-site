# Scout

Scout is a Windows 11 launcher for finding files, apps, links, and saved
workspaces from one keyboard shortcut.

- [Website](https://adilzubair.github.io/scout-site/)
- [Download the Windows beta](https://github.com/adilzubair/scout-site/releases/tag/v0.1.0-beta.2)

Download `Scout-Setup.exe`, run it without admin access, and press
**Ctrl+Alt+Space** to open Scout. Setup creates Start menu shortcuts for Scout
and its uninstaller. The portable `Scout-win-x64.zip` is also available.

This beta is unsigned, so Windows may show an unknown-publisher or SmartScreen
warning. Updates are manual; there is no automatic updater.

This repository contains the public website and release downloads.

## Subdomain redirect

`vercel.json` configures a separate Vercel deployment to forward all requests to
`https://adilzubair.github.io/scout-site/` with an HTTP 308 permanent redirect.
Connect `scout.muhamedadil.com` to the `scout-redirect` project. DNS is managed by
Vercel; the portfolio remains attached to the main domain.
