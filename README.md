# Mira

Working Student, Evaluation Engineering & Product at [@userlike](https://github.com/userlike).
Computational Humanities and linguistics and NLP, Uni Köln.

I build and run a LLM evaluation system for a customer-communication AI product:
dataset design, LLM-as-judge rubrics, judge calibration, and the model comparisons behind
provider decisions. Built on Langfuse. Four eval datasets so far, including a τ²-bench
adaptation and the paired significance testing behind provider and prompt change decisions.

Also into immutable Linux desktops — daily-driving
[bazzite-dx](https://github.com/ublue-os/bazzite-dx) for container-native dev.

And [Langfuse Cloud Platform](https://github.com/langfuse/langfuse) for an open source AI engineering platform with LLM evals, observability, metrics, prompt management, playground, datasets.

## Selected work

**[Plant-Identifier](https://github.com/mira-sp/Plant-Identifier-Webapp)** — Local-first plant identification. A vision model (qwen2.5vl:7b via Ollama) runs on your own machine, so photos never leave the device. Two-stage pipeline (classify → describe), with one zod schema serving as TypeScript types, runtime validation and Ollama's constrained output format. The eval harness runs the exact production code over iNaturalist, non-plant and personal photo splits, matches names via the GBIF backbone so synonyms count as correct, and reports top-1/top-3 accuracy, schema validity, abstention, latency and calibration (ECE plus a threshold table that decides when the app shows several candidates instead of one). Next.js 16 · React 19 · TypeScript · Vitest · GitHub Actions.

**[german-hate-speech-classification](https://github.com/mira-sp/german-hate-speech-classification)** — GBERT vs mBERT vs HateBERT on GermEval 2018, 5-fold stratified CV. GBERT wins at F1 0.808 ±0.020; HateBERT drops 14 points because hate-speech pretraining doesn't survive a language switch. Favourite ablation: lowercasing hurts German, because capitalization carries semantic signal.

**[vinted-checker](https://github.com/mira-sp/vinted-checker)** — Local app that checks whether a photo, e.g. from a Vinted listing, matches a known product from fast-fashion shops like Shein or Temu. Three signals get merged and ranked: CLIP embeddings (transformers.js) for visually similar products, perceptual hashing (sharp-phash) for near-identical copies, and optional reverse image search via Google Cloud Vision. Fastify · better-sqlite3 · sharp, listening only on 127.0.0.1 with all data stored locally.

**[GeoGuesserClone](https://github.com/mira-sp/GeoGuesserClone)** — Location-guessing Android game with real-time multiplayer. Kotlin/MVVM client (Room, Retrofit2, osmdroid) against a Node/Express backend: PostgreSQL + PostGIS, JWT auth, REST plus Socket.IO for live rounds. Street-level imagery from Mapillary with a bitmap fallback. Runs end to end on free-tier infrastructure.

**[Gender-Korpus](https://github.com/mira-sp/Gender-Korpus)** — Short analysis of 684k tokens of German text (18th–20th century), 29k of them gender-labelled, with spaCy POS tagging over the labelled subset. Built for a university course. Label split: Mann 61% · Frau 35% · gender-neutral 4%.

## Stack

**Eval & LLM** Langfuse · Ragas · OpenAI SDK (async · structured output · streaming) · LLM-as-judge design · multi-provider routing (OpenRouter · Bedrock · Azure) · Pydantic · zod · Ollama · transformers.js

**Engineering** Python · Django (ORM · admin · management commands · Celery) · FastAPI · Fastify · Postgres/SQL · SQLite · pytest · Vitest · Docker · TypeScript / React / Next.js · Kotlin · PyTorch · Transformers

[LinkedIn](https://www.linkedin.com/in/mira-speier) · [Mail](mailto:mira.speier@web.de)
