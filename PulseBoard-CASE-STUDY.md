# 📊 PulseBoard — Revenue & Ops Intelligence

> Un dashboard care nu doar afișează date, ci le interpretează cu AI și propune acțiuni.
> A dashboard that doesn't just display data — it interprets it with AI and suggests actions.

![status](https://img.shields.io/badge/status-live-success) ![stack](https://img.shields.io/badge/React-Vite-blue) ![ai](https://img.shields.io/badge/AI-Anthropic-orange) ![lang](https://img.shields.io/badge/RO%2FEN-bilingv-yellow)

---

## 🇷🇴 Română

### Problema

Un founder solo de micro-SaaS avea vânzările împrăștiate în trei locuri: Stripe, un export de Shopify și un Google Sheet pe care îl actualiza manual. La sfârșitul fiecărei săptămâni pierdea o oră încercând să răspundă la o întrebare simplă — *„merge mai bine sau mai prost decât săptămâna trecută, și de ce?"* — fără să aibă timp să devină analist de date.

### Soluția

**PulseBoard** transformă orice export tabelar într-un panou de control clar, în câteva secunde:

- **Import real** — încarci un CSV sau lipești linkul unui Google Sheet public; coloanele (dată, venit, comenzi) sunt detectate automat.
- **KPI-uri vii** — venit, comenzi, clienți noi și rată de conversie, fiecare cu variația față de perioada anterioară.
- **Detectare de anomalii** — zilele neobișnuite (scăderi sau vârfuri) sunt marcate automat pe grafic, pe baza unui scor statistic.
- **Briefing executiv scris de AI** — un model citește metricile și scrie un rezumat în limbaj natural, **plus 2–3 acțiuni concrete prioritizate**.
- **Comparație de perioade** și **export** al raportului cu un click.
- Totul **bilingv RO/EN**, design dark editorial.

### Rezultatul

Întrebarea de o oră devine un răspuns de zece secunde. Founderul deschide PulseBoard, vede pe loc unde stă, citește briefing-ul AI și știe exact ce să facă în continuare — fără să atingă o formulă.

### Stack

`React 18` · `Vite` · `Recharts` · `Anthropic API` (cu fallback determinist offline) · `JavaScript`

---

## 🇬🇧 English

### The problem

A solo micro-SaaS founder had sales scattered across three places: Stripe, a Shopify export, and a Google Sheet they updated by hand. Every week's end cost them an hour trying to answer one simple question — *"are we doing better or worse than last week, and why?"* — with no time to become a data analyst.

### The solution

**PulseBoard** turns any tabular export into a clear control panel in seconds:

- **Real import** — upload a CSV or paste a public Google Sheet link; columns (date, revenue, orders) are auto-detected.
- **Live KPIs** — revenue, orders, new customers and conversion rate, each with its change versus the prior period.
- **Anomaly detection** — unusual days (drops or spikes) are flagged automatically on the chart via a statistical score.
- **AI-written executive briefing** — a model reads the metrics and writes a natural-language summary, **plus 2–3 concrete, prioritized actions**.
- **Period comparison** and one-click **report export**.
- Fully **bilingual RO/EN**, dark editorial design.

### The result

The one-hour question becomes a ten-second answer. The founder opens PulseBoard, instantly sees where things stand, reads the AI briefing, and knows exactly what to do next — without touching a formula.

### Stack

`React 18` · `Vite` · `Recharts` · `Anthropic API` (with deterministic offline fallback) · `JavaScript`

---

## 🧠 Decizii de design / Design decisions

- **AI cu fallback** — când API-ul nu e disponibil, un motor local generează briefing-ul și acțiunile, deci demo-ul nu „cade" niciodată în fața unui recruiter sau client.
- **Date determinist-generate (seed)** — datele demo sunt coerente și re-rulabile, nu random la fiecare render.
- **Detectare anomalii cu z-score** — simplu, transparent, fără dependențe externe.

> _Construit ca piesă de portofoliu. Datele demo sunt simulate; importul funcționează cu date reale. / Built as a portfolio piece. Demo data is simulated; import works with real data._
