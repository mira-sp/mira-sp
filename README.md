# Mira

Working Student, Evaluation Engineering & Product at [@userlike](https://github.com/userlike).
Computational linguistics and NLP, Uni Köln.

I build and run a LLM evaluation system for a customer-communication AI product:
dataset design, LLM-as-judge rubrics, judge calibration, and the model comparisons behind
provider decisions. Built on Langfuse. Four eval datasets so far, including a τ²-bench
adaptation and the paired significance testing behind provider and prompt change decisions.

Also into immutable Linux desktops — daily-driving
[bazzite-dx](https://github.com/ublue-os/bazzite-dx) for container-native dev.

And [Langfuse Cloud Platform](https://github.com/langfuse/langfuse) for an open source AI engineering platform with LLM evals, observability, metrics, prompt management, playground, datasets.

## Selected work

- **[german-hate-speech-classification](https://github.com/mira-sp/german-hate-speech-classification)**
  — GBERT vs mBERT vs HateBERT on GermEval 2018, 5-fold stratified CV. GBERT wins at
  F1 0.808 ±0.020; HateBERT drops 14 points because hate-speech pretraining doesn't survive a
  language switch. Favourite ablation: lowercasing *hurts* German — capitalization carries
  semantic signal.

- **[GeoGuesserClone](https://github.com/mira-sp/GeoGuesserClone)** — Location-guessing Android
  game with real-time multiplayer. Kotlin/MVVM client (Room, Retrofit2, osmdroid) against a
  Node/Express backend: PostgreSQL + PostGIS, JWT auth, REST plus Socket.IO for live rounds.
  Street-level imagery from Mapillary with a bitmap fallback. Built to run on free-tier
  infrastructure end to end with Google SDK. 

- **[Gender-Korpus](https://github.com/mira-sp/Gender-Korpus)** — Short Analysis of a 684k tokens of German text
  (18th–20th c.), 29k gender-labelled, spaCy POS tagging over the labelled subset. For university purposes.
  Mann 61% / Frau 35% / genderneutral 4%.

- **[Plant-Identifier-Webapp](https://github.com/mira-sp/Plant-Identifier-Webapp)** —  photo in, structured plant profile out. Camera capture via `getUserMedia`,
  Leaflet for origin regions. Currently in work



## Stack

**Eval & LLM** Langfuse · Ragas · OpenAI SDK (async · structured output · streaming) ·
LLM-as-judge design · multi-provider routing (OpenRouter · Bedrock · Azure) · Pydantic

**Engineering** Python · Django (ORM · admin · management commands · Celery) · FastAPI ·
Postgres/SQL · pytest · Docker · TypeScript / React / Next · Kotlin · PyTorch · Transformers

[LinkedIn](https://www.linkedin.com/in/mira-speier/) · [Mail](mailto:speiermia@gmail.com)
