<div align="center">

# 📊 PulseBoard

### Revenue & Ops Intelligence — un dashboard care interpretează datele, nu doar le afișează

[![status](https://img.shields.io/badge/status-live-success?style=flat-square)](https://laurandreea10.github.io/PulseBoard/)
[![React](https://img.shields.io/badge/React-18-61dafb?style=flat-square&logo=react&logoColor=white)](https://react.dev)
[![Vite](https://img.shields.io/badge/Vite-build-646cff?style=flat-square&logo=vite&logoColor=white)](https://vitejs.dev)
[![Recharts](https://img.shields.io/badge/Recharts-charts-22b5bf?style=flat-square)](https://recharts.org)
[![AI](https://img.shields.io/badge/AI-Anthropic-e8b84b?style=flat-square)](https://www.anthropic.com)
[![lang](https://img.shields.io/badge/RO%2FEN-bilingv-fbbf24?style=flat-square)]()

> **Cele mai multe dashboard-uri răspund la „ce s-a întâmplat?”. PulseBoard răspunde la „ce s-a întâmplat, de ce și ce fac acum?”.**
> *Most dashboards answer "what happened?". PulseBoard answers "what happened, why, and what do I do now?".*

[🔴 Live Demo](https://laurandreea10.github.io/PulseBoard/) · [📄 Case Study](https://laurandreea10.github.io/codepen-portfolio/projects/pulseboard.html)

</div>

---

## 🇷🇴 Română

### 🎯 Originea proiectului

Pentru un founder solo de micro-SaaS, datele de business trăiesc în trei locuri în același timp: Stripe pentru încasări, un export de Shopify pentru comenzi, un Google Sheet actualizat manual pentru rest. Întrebarea de la finalul fiecărei săptămâni — *„mergem mai bine sau mai prost decât săptămâna trecută, și de ce?”* — costă o oră de copiat coloane.

**PulseBoard** transformă orice export tabelar într-un răspuns clar, în câteva secunde — și adaugă stratul pe care dashboard-urile obișnuite îl ratează: un briefing scris de AI care îți spune ce să faci în continuare.

### ✨ Funcționalități

- 📥 **Import real de date** — drag & drop CSV sau link de Google Sheet public; coloanele (dată, venit, comenzi, clienți, vizite) detectate automat, în RO sau EN.
- 📈 **KPI-uri vii** — venit, comenzi, clienți noi, rată de conversie, fiecare cu variația față de perioada anterioară.
- 🚨 **Detectare de anomalii** — zilele neobișnuite marcate automat pe grafic (z-score), roșu pentru scădere, verde pentru vârf.
- 🤖 **Briefing executiv scris de AI** — rezumat în limbaj natural **plus 2–3 acțiuni concrete prioritizate**.
- 🔀 **Comparație de perioade** — suprapune perioada anterioară pe grafic.
- 📤 **Export** al raportului cu un click.
- 🌍 **Bilingv RO/EN**, design dark editorial.

### 🛠️ Tehnologii

`React 18` · `Vite` · `Recharts` · `Anthropic API` (cu fallback determinist offline) · `JavaScript` · `GitHub Pages`

---

## 🇬🇧 English

### 🎯 Project origin

For a solo micro-SaaS founder, business data lives in three places at once: Stripe for revenue, a Shopify export for orders, a hand-updated Google Sheet for the rest. The end-of-week question — *"are we doing better or worse than last week, and why?"* — costs an hour of copying columns.

**PulseBoard** turns any tabular export into a clear answer in seconds — and adds the layer ordinary dashboards miss: an AI-written briefing that tells you what to do next.

### ✨ Features

- 📥 **Real data import** — drag & drop CSV or paste a public Google Sheet link; columns (date, revenue, orders, customers, visits) auto-detected, in RO or EN.
- 📈 **Live KPIs** — revenue, orders, new customers, conversion rate, each with its change vs the prior period.
- 🚨 **Anomaly detection** — unusual days flagged automatically on the chart (z-score), red for drops, green for spikes.
- 🤖 **AI-written executive briefing** — natural-language summary **plus 2–3 concrete, prioritized actions**.
- 🔀 **Period comparison** — overlays the previous period on the chart.
- 📤 **One-click report export**.
- 🌍 **Bilingual RO/EN**, dark editorial design.

### 🛠️ Tech

`React 18` · `Vite` · `Recharts` · `Anthropic API` (with deterministic offline fallback) · `JavaScript` · `GitHub Pages`

---

## 🧠 Decizii de design / Design decisions

| Decizie / Decision | De ce / Why |
|---|---|
| **AI cu fallback local** | Demo-ul nu „cade” niciodată — motorul local generează briefing-ul când API-ul nu răspunde. / The demo never breaks — a local engine generates the briefing when the API is down. |
| **Date demo determinist-generate (seed)** | Coerente și re-rulabile, nu random la fiecare render. / Coherent and replayable, not random per render. |
| **Detectare anomalii cu z-score** | Simplu, transparent, fără dependențe externe. / Simple, transparent, zero external dependencies. |

---

## 🚀 Îmbunătățiri planificate / Planned improvements

- [ ] Detectare de anomalii cu **sezonalitate** (normalizare pe ziua săptămânii) / Anomaly detection with **seasonality**
- [ ] **Conectori direcți** (Stripe, Shopify) în locul exportului manual / **Direct connectors** instead of manual export
- [ ] **Briefing programat** trimis automat luni dimineața / **Scheduled briefing** auto-sent Monday morning
- [ ] Export **PDF/PNG** al întregului dashboard / Full-dashboard **PDF/PNG** export

---

## 🗺️ Roadmap

| Versiune | Status | Conținut |
|---|---|---|
| **v1** | ✅ | KPI-uri, grafice, briefing AI, RO/EN |
| **v2** | ✅ | Import CSV/Sheet, acțiuni AI, anomalii, comparație, export |
| **v3** | 🔜 | Conectori direcți, sezonalitate, briefing programat |

---

## ⚙️ Rulare locală / Local setup

```bash
git clone https://github.com/LaurAndreea10/PulseBoard.git
cd PulseBoard
npm install
npm run dev
```

> Importul de Google Sheet cere ca sheet-ul să fie publicat ca CSV (*Fișier → Partajează → Publică pe web → CSV*). Upload-ul de CSV local merge mereu. / Google Sheet import requires the sheet to be published as CSV. Local CSV upload always works.

---

<div align="center">

**Laura Andreea** · [GitHub](https://github.com/LaurAndreea10) · construit ca piesă de portofoliu / built as a portfolio piece

⭐ Dacă îți place, lasă o stea / If you like it, leave a star

</div>
