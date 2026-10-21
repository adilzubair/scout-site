# Contributing to the Scout website

This repository contains Scout's static website and public Windows downloads.
Application code and its build/test instructions live in
[`adilzubair/scout`](https://github.com/adilzubair/scout).

## Make a website change

1. Make the change in
   [`scout/website/dist/`](https://github.com/adilzubair/scout/tree/main/website/dist),
   the maintained website source. Keep the copy in this repository in sync.
2. Preview the static site using the instructions in [README.md](README.md).
3. Check desktop and narrow mobile layouts, navigation, example switching,
   keyboard focus, FAQ disclosures, images, fonts, and download links. The core
   content and navigation should remain usable without JavaScript.
4. Keep asset paths relative for the GitHub Pages project URL. Preserve font
   license notices and `vercel.json`.
5. Describe the change and what you checked in your pull request. Include
   screenshots for visible changes.

The site needs no application build or Node.js dependencies. Never commit
personal files, diagnostic output, model weights, local runtimes, credentials,
or Windows release binaries to Git.

## Publish website updates

Copy only the contents of `scout/website/dist/` into this repository's root.
Review the diff before committing; preserve this repository's README,
contribution guide, `.github/` files, `.gitignore`, and `vercel.json`. Remove
obsolete site assets only after checking that no page or stylesheet uses them.

A push to `main` automatically deploys the site on Vercel. Verify
`https://scout.muhamedadil.com/` after deployment and check relative paths at
`https://adilzubair.github.io/scout-site/` when updating shared assets.

## Update download links

Build and verify a release in the application repository using its own
contribution and packaging instructions. Upload the verified installer,
portable ZIP, and matching SHA-256 files to a GitHub Release in `scout-site`.
Record the application source commit in the release notes; this repository's
automatic source archives contain website files.

Before changing the site's advertised version, check that the release is
published and all four download assets exist. Update the installer, ZIP,
checksum links, release links, and version labels together in both website
copies and this README. Keep older releases available for existing links.

## Report a problem

Use this repository's issues for website content, layout, accessibility, or
broken links. Report launcher behavior and Windows installation problems in
the [application repository](https://github.com/adilzubair/scout/issues).
