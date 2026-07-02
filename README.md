## 👋 hey, I'm Enzo

I build slightly obsessive infrastructure for **multilingual & translation data** — the unglamorous plumbing that turns _cursed XML from 2004_ into things you can actually reason about. If you've ever opened a TMX file and quietly closed it again, we should talk.

Mostly a **Python** dev. Currently **learning Rust in public**, one over-engineered domain model at a time. The rule: I don't merge what I can't explain.

## 🔭 what I'm building

**[Observatory](https://github.com/EnzoAgosta/observatory) — flagship, and my current rabbit hole** 🐇
A lakehouse for multilingual data that treats a string's _identity_ and the _facts about it_ as two different things. It's basically **event sourcing for translation memory**: the observation log is the source of truth, and the classic source→target TM is just a view you _derive_. Content-addressed atoms, append-only observations, Lance + DuckDB under the hood. Very much **R&D first** — a reimagining of what translation data even _is_, and a product only maybe-someday.

**[hypomnema](https://github.com/EnzoAgosta/hypomnema) — the pandas of TMX**
A type-safe, dependency-free Python library for TMX 1.4B. TMX is 25 years old, every CAT tool emits it, and the Python ecosystem still had _nothing_ that gave you a typed, validated, round-trippable domain model without making you think about XML internals. Now it does. `mypy --strict`, zero required deps, and it loses nothing on a round-trip — anything it doesn't model is preserved verbatim rather than silently dropped.

**[tournament-eval](https://github.com/EnzoAgosta/tournament-eval) — let the models rank each other**
Circular peer-ranking for LLMs, born from fine-tuning translation models with no gold answer to grade against. Instead of trusting one ranker's blind spots, a whole panel ranks each other's work — authorship hidden behind aliases — and their biases become _signal_ instead of noise. Order-invariant aggregation, full reasoning capture, model-agnostic.

> Spot the theme? Faithful data models for multilingual stuff, and a deep suspicion of tools that lose or flatten information. I have a type.

## 🧰 stack-ish

- **Python** 🐍 — home turf. 3.13+, `match`/`case`, frozen slotted dataclasses, generics-that-don't-say-`TypeVar`, and `mypy --strict` or it didn't happen.
- **Rust** 🦀 — the new hotness I'm actively learning. A lot of the heavy lifting happens in concert with AI, but I overlook every architecture decision, rewrite the parts I don't like, and am stubborn about actually _understanding_ it rather than cargo-culting.
- **JS / TS / React** — enough to be dangerous (thanks, day job). Not going to pretend it's production-grade artistry.
- **AI & data** — Lance, DuckDB, embeddings, LLM-eval plumbing, Pydantic AI.

## 🪧 hills I will (cheerfully) die on

- A string's **identity** and the **facts about it** are different things, and conflating them ruins everything downstream. See: every TM ever built.
- A round-trip that loses data is a **bug**, not a "limitation."
- **Dumb primitives > clever frameworks.** Push policy out to the caller; keep the core boring and total.
- `Any` is a confession, not a type.
- **Reproducibility isn't optional** — if the same input gives a different id, you've got nothing.

## 📊 the obligatory widgets

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=EnzoAgosta&show_icons=true&hide_border=true&theme=tokyonight" alt="Enzo's GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=EnzoAgosta&layout=compact&hide_border=true&theme=tokyonight" alt="Top languages" />
</p>

## 📫 find me

- 🐙 GitHub: [@EnzoAgosta](https://github.com/EnzoAgosta)
- 💼 LinkedIn: [@EnzoAgosta](hhttps://www.linkedin.com/in/agosta-enzo/)
