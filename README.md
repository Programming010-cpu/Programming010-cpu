````markdown
<!-- Badges -->
![License](https://img.shields.io/github/license/zmyrna/zmyrna)
![Build](https://img.shields.io/github/actions/workflow/status/zmyrna/zmyrna/ci.yml?label=build)
![Release](https://img.shields.io/github/v/release/zmyrna/zmyrna)

# Zmyrna • 100 Moments Minted
*A protocol that mints nostalgia, one token at a time.*

> “Some winters are loud enough to echo for years.” – *River‑Road Nocturne*

---

## ✨ What is Zmyrna?
Zmyrna is an **art‑backed ERC‑721 collection** binding autobiographical vignettes to on‑chain metadata.  
Only **100 tokens** exist; each carries a short prose fragment and a generative oil‑canvas image.

| Feature | Status |
|---------|--------|
| Fully on‑chain metadata | ✅ |
| Story‑image pairing via IPFS | ✅ |
| DAO‑gated narrative extensions | 🚧 *(roadmap Q4 2025)* |

---

## 🔧 Quick start

```bash
# Clone & run the website locally
git clone https://github.com/zmyrna/zmyrna.git
cd zmyrna/apps/web
pnpm install          # or npm / yarn
pnpm run dev          # Next.js preview at http://localhost:3000
````

```bash
# Test smart‑contracts
cd ../../contracts
forge test -vv
```

---

## 🖼️ Screenshots

<p align="center">
  <img src="docs/screenshot_hero.png" width="640" alt="River‑Road Nocturne hero section"/>
</p>

---

## 📚 Architecture

```
zmyrna/
  apps/
    web/            # Next.js + Tailwind + shadcn/ui
  contracts/
    ZmyrnaToken.sol # ERC‑721 + EIP‑2981 royalties
  packages/
    ui/             # Shared React components
    config/         # Hardhat & Forge configs
```

* Solidity 0.8.26 • Foundry for tests • IPFS pinning via web3.storage \*

---

## 🤝 Contributing

1. Fork → `feat/my-idea` branch.
2. `pnpm lint && pnpm test` must pass.
3. Open a PR—story‑driven code comments encouraged.

See issues tagged **`good first story`** for starter tasks.

---

## 🗺️ Roadmap

| Milestone                           | ETA         |
| ----------------------------------- | ----------- |
| Governance snapshot launch          | **Q3 2025** |
| Story‑submission CLI release        | **Q3 2025** |
| Volume II (tokens 101‑200) DAO vote | **Q4 2025** |
| On‑chain generative cover art       | **2026**    |

---

## 📝 License

MIT © 2025‑2077 Zmyrna.
*It’s not magic—it’s “protocol.”*

```
```
