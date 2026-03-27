# Swarm — Project Tracker

**Client:** Swarm (American-made autonomous drone systems, defense tech)
**GitHub:** `ffgroup-8/swarm` → https://github.com/ffgroup-8/swarm
**Local:** `~/Desktop/Git Repo/Swarm/index.html`
**Live:** https://ffgroup-8.github.io/swarm/

---

## Master Rules

Follow all rules in `../_Project Tracker Master/CLAUDE.md`. That file is the source of truth for:
- Box hierarchy (`seo-box` → `content-created-box` as siblings)
- CSS patterns (green seo-box, blue content-created-box, dark mode)
- Status pill system (6 categories)
- SEO standards
- Push-automatically rule
- Content writing standard (actual copy, not design annotations)

**Pipeline:** If you add a new pattern here that isn't in Master, also apply it to `../_Project Tracker Master/index.html` and commit both.

---

## Current Progress

| Category        | Progress |
|-----------------|----------|
| Design          | (check tracker) |
| Dev             | (check tracker) |
| SEO             | (check tracker) |
| Content Input   | (check tracker) |
| Sanity Dev      | (check tracker) |
| Content Created | 0% (0/11 pages complete) |

---

## Pages (11 content pages)

| # | Page | Slug | Content Created |
|---|------|------|-----------------|
| 1 | 🏠 Home | `/` | ⬜ needed |
| 2 | 🛩️ Drones (Gen2 Platform) | `/drones` | ⬜ needed |
| 3 | 💻 Software | `/software` | ⬜ needed |
| 4 | ⚡ Capabilities | `/capabilities` | ⬜ needed |
| 5 | 🎯 Training Systems | `/training` | ⬜ needed |
| 6 | 👥 Team | `/team` | ⬜ needed |
| 7 | 📰 Press (Content Hub) | `/press` | ⬜ needed |
| 8 | ❓ FAQs | `/faqs` | ⬜ needed |
| 9 | 📞 Contact | `/contact` | ⬜ needed |
| 10 | 🔍 SEO: Drone Swarm Technology | `/drone-swarm-technology` | ⬜ needed |
| 11 | 🔍 SEO: Counter-UAS Solutions | `/counter-uas` | ⬜ needed |
| 12 | 🔍 SEO: American-Made Drones | `/american-made-drones` | ⬜ needed |
| 13 | 🔍 SEO: Attritable Drone Systems | `/attritable-drones` | ⬜ needed |
| — | Knowledge Base sections | — | n/a |

---

## Swarm-Specific Notes

- Dark mode seo-box was previously broken (used grey tones instead of green). **Fixed** — now uses `#0d1f14` background, `#1a4d30` border, `#34d399` title color, matching master standard
- All seo-boxes were previously in `<table>` format — **converted** to `<p><strong>Label:</strong> value</p>` format
- Brand voice: Precise, technical, confident. Defense/government audience. No hype.

---

## Content Module Template

```html
<p><strong>📌 Module 1 — Hero</strong></p>
<ul>
  <li><strong>Headline:</strong> ...</li>
  <li><strong>Subheadline:</strong> ...</li>
  <li><strong>CTA:</strong> ...</li>
</ul>
```

After adding content for a page:
1. Mark Content Created pill `completed` in both nav-item AND sitemap node
2. Recalculate `data-target` on Content Created progress bar: `(N / 11 * 100).toFixed(0)%`
3. Commit and push automatically
