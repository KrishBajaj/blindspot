# Blindspot source for GitHub

This repository contains the Blindspot website source. The live Site is hosted privately in ChatGPT Sites. Its pilot request form writes to a server-side R2 bucket; GitHub Pages cannot run this worker or store submissions.

## Open in GitHub Codespaces
Create a new GitHub repository named `blindspot`, upload the files in this folder (including `worker/index.js`), then select **Code → Codespaces → Create codespace on main**. Open `worker/index.js` to edit the site.

## Run locally in Codespaces
Use Cloudflare Wrangler in a separate Cloudflare project if you want to run the Worker outside ChatGPT Sites. That requires configuring an R2 bucket binding named `BUCKET`. Do not publish an untested form or remove the server endpoint without adjusting the page.

## Keep the live Site current
This GitHub copy is not automatically synced to the ChatGPT Site. Edits here need to be ported and redeployed to the original Site, or you can move hosting to a Cloudflare Worker of your own.
