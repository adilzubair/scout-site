# Scout

Scout is a Windows 11 launcher for finding files, opening apps and links,
controlling everyday PC settings, and reopening saved workspaces from one
keyboard shortcut.

- [Website](https://scout.muhamedadil.com/)
- [Download the Windows beta](https://github.com/adilzubair/scout-site/releases/tag/v0.1.0-beta.2)

Download `Scout-Setup.exe`, run it without admin access, and press
**Ctrl+Alt+Space** to open Scout. Setup creates Start menu shortcuts for Scout
and its uninstaller. The portable `Scout-win-x64.zip` is also available.

This beta is unsigned, so Windows may show an unknown-publisher or SmartScreen
warning. Updates are manual; there is no automatic updater.

This repository contains the public website and release downloads.

The website uses self-hosted Uncut Sans and Inter. Their SIL Open Font Licenses
are included in `fonts/UncutSans-LICENSE.txt` and `fonts/LICENSE.txt`.

## Custom domain hosting

Vercel serves this repository's static website directly at
`https://scout.muhamedadil.com/`. The `scout-redirect` project retains its original
name but no longer forwards visitors to GitHub Pages. DNS and HTTPS are managed
by Vercel. Changes pushed to `main` automatically deploy the website.

GitHub Pages remains available at `https://adilzubair.github.io/scout-site/`.
