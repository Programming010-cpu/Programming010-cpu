
## 1 · Principles before prose

| Principle                    | What it means for Zmyrna                                                                                                  |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **Clarity first**            | Assume newcomers land here from Google, not from your Twitter thread. Write the TL;DR in ≤ 3 sentences.                   |
| **Front‑load the wow**       | Show, don’t tell—one hero screenshot or GIF beats 20 lines of text.                                                       |
| **Self‑contained setup**     | A 30‑second “clone → run” path turns lurkers into contributors. Script it if possible.                                    |
| **Badge‑driven credibility** | Shields.io badges for license, build status, and latest release give instant trust signals.                               |
| **Story‑echo**               | Mirror the poetic tone of your site only in the tagline and screenshots; keep installation and API docs strictly literal. |
| **Progressive detail**       | Start with 100‑level “why,” then 200‑level “how,” then 300‑level “behind the curtain.” Readers drop off in that order.    |

---

## 2 · README skeleton (Markdown)

````markdown
<!-- Badges -->
![License](https://img.shields.io/github/license/yourname/zmyrna)
![Build](https://img.shields.io/github/actions/workflow/status/yourname/zmyrna/ci.yml?label=build)
![Release](https://img.shields.io/github/v/release/yourname/zmyrna)

# Zmyrna • 100 Moments Minted
*A protocol that mints nostalgia, one token at a time.*

> “Some winters are loud enough to echo for years.” – *River‑Road Nocturne*

---

## ✨ What is Zmyrna?
Zmyrna is an **art‑backed ERC‑721 collection** that binds autobiographical vignettes to on‑chain metadata.  
Each of the 100 tokens is an immutable snapshot of a half‑remembered night—bikes, neon rivers, contraband ramen.

| Feature | Status |
|---------|--------|
| Fully on‑chain metadata | ✅ |
| Story‑image pairing via IPFS | ✅ |
| DAO‑gated narrative extensions | 🚧 *(roadmap Q4 2025)* |

---

## 🔧 Quick start
```bash
git clone https://github.com/yourname/zmyrna.git
cd zmyrna
pnpm install      # or npm / yarn
pnpm run dev      # local Next.js preview
````

For smart‑contract testing:

```bash
forge test -vv
```

---

## 🖼️ Screenshots

<p align="center">
  <img src="docs/screenshot_hero.png" width="600" alt="River‑Road Nocturne hero section"/>
</p>

---

## 📚 Architecture

```
apps/
  web/          # Next.js front‑end
contracts/
  ZmyrnaToken.sol
packages/
  ui/           # Shared React components (Tailwind + shadcn/ui)
```

* Solidity 0.8.26
* Foundry for tests & deployment
* IPFS pinning via web3.storage

---

## 🤝 Contributing

1. Fork the repo & create a branch (`feat/my-idea`).
2. Run `pnpm lint && pnpm test`.
3. Submit a PR—stories as code comments encouraged.

Need inspiration? Check the open issues tagged **`good first story`**.

---

## 🗺️ Roadmap

* **Q3 2025** – Launch governance snapshot; open source story‑submission CLI.
* **Q4 2025** – DAO votes on the *Volume II* expansion (tokens 101‑200).
* **2026** – On‑chain generative cover art.

---

## 📝 License

MIT © 2025‑2077 Zmyrna.
*It’s not magic—it’s “protocol.”*

```

---

## 3 · Polish moves (“招法”)

1. **Auto‑generated TOC**  
   Add `<!-- toc -->` markers or use `markdown‑toc` to keep section links fresh.

2. **GIF demo**  
   Record a 5‑second loom of the mint flow; compress with `gifsicle --optimize`.

3. **Version badge from NPM**  
   If you publish a front‑end package, add `![npm](https://img.shields.io/npm/v/@zmyrna/ui)`.

4. **CI check for broken links**  
   Use `lychee‑action` so every PR runs `lychee --markdown`.

5. **“Copy code” buttons**  
   For the quick‑start snippet, embed `[copy]` buttons via `markdown‑code‑embed`.

6. **Commit message style guide**  
   Link to `CONTRIBUTING.md` with Conventional Commits or Gitmoji; helps auto‑changelog later.

---

### Final tip
Treat the README as a **living landing page**: each release tag should tweak the screenshot and roadmap. If a stranger can’t answer *“What problem does this solve and how do I try it in under five minutes?”* the README still needs pruning.

Plug the skeleton above into `README.md`, sprinkle in your own screenshots, and you’re launch‑ready.
```
