# Vault Solutions

Chrome extensions that save, filter, and organize the things you'd otherwise lose — search results, AI conversations, saved pages, and copied prompts. Each product is self-contained, Manifest V3, and stores your data locally on your own device.

| Product | What it does | Folder |
|---|---|---|
| **Refinasearch** | Reorders and filters Google, Bing, and DuckDuckGo results — boost the sources you trust, hide the ones you don't, in one click. | [`refinasearch/`](./refinasearch) |
| **Prompt Vault** | Automatically saves your AI conversations (ChatGPT, Claude, Gemini, Copilot, Perplexity) as local files. | [`prompt-vault/`](./prompt-vault) |
| **PageKeeper** | One floating button that saves any page as a bookmark, screenshot, or full single-file HTML archive. | [`pagekeeper/`](./pagekeeper) |
| **Prompt Keeper** | Automatically saves prompts you copy while working with AI image/video generators. | [`prompt-keeper/`](./prompt-keeper) |

## Shared design principles

- **Local-first.** Every product stores your data in your browser's local storage — nothing is uploaded to a Vault Solutions server. The only network request any of these extensions makes is a license check against [ExtensionPay](https://extensionpay.com), used to process one-time Founder purchases via Stripe.
- **Manifest V3.** All four are built on the current extension platform, with no remotely-hosted code and no `eval`.
- **Free tier + one-time Founder purchase.** Each product has a genuinely useful free tier, with a single lifetime "Founder" purchase (not a subscription) to unlock the rest — priced and structured independently per product.

## Repository layout

Each product folder is a complete, independent Chrome extension — `manifest.json` at its own root, ready to be zipped and uploaded to the Chrome Web Store as-is, or loaded unpacked for local development (`chrome://extensions` → Developer mode → Load unpacked → select the product folder).

## Privacy

Each product publishes its own privacy policy, linked from its Chrome Web Store listing. In short: local storage only, no analytics, no tracking, and no data collection beyond what's strictly needed for the product's stated purpose.

## License

See [LICENSE.md](./LICENSE.md). All rights reserved — this is proprietary, commercial software; the source is here for development and transparency, not for redistribution or reuse.

## Contact

lineinbetween@gmail.com
