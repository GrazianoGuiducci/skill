# THIA Skill Repository — Snapshot v3 (2026-02-26)

Complete catalog of skills from the THIA system, organized by the **3-Plane Taxonomy**.

> **Snapshot**: This repo is synced periodically from THIA production. Not a live mirror.

## 3-Plane Taxonomy

Skills are organized by **where they live**, not just what they do:

| Plane | Description | Environments | Count |
|:------|:------------|:-------------|:------|
| **Plane 1** — Cognitive | How the system *thinks*. Pure inference angles. No infrastructure bindings. | Claude.ai + THIA repo | 17 |
| **Plane 2** — Operative | How the system *acts*. Emit commands, talk to VPS/APIs/filesystem. | THIA repo only | 11 |
| **Plane 3** — Bridges | Translate between planes. Connect nodes. | Claude.ai + THIA repo | 3 |
| **Conductor** | Routes requests to the appropriate skills per environment. | Both (different versions) | 2 |

> **Kernel MM** (Plane 0) is not a skill — it's the invariant Field encoded in the system prompt / userPreferences.

## Format

Each skill is stored as `agent_skills_[name].md` containing the complete SKILL.md content from the source directory structure. This flat format enables:

- Direct file inclusion in agent systems
- Simple version control and Git tracking
- Easy deployment to multiple environments
- Clear skill indexing and catalog management

## Two Channels

Skills are distributed through two channels depending on your environment:

### Channel 1 — Coder (Claude Code, Cursor, Windsurf, etc.)

Copy `agent_skills_*.md` files directly into your project (e.g., `.agent/skills/`). Full THIA-format with triggers, metadata, and collaboration hooks. Plane 1 skills are portable — Plane 2 require THIA infrastructure.

### Channel 2 — Chat AI (Claude.ai, ChatGPT, Gemini)

Use the **[Thinker Pack](thinker-pack/)**: Kernel MM + 17 cognitive skills formatted for AI chat interfaces. Paste the Kernel into User Preferences, then add individual skills to your projects.

See [thinker-pack/README.md](thinker-pack/README.md) for setup instructions.

## How to Use

1. **Include individual skills**: Copy any `agent_skills_*.md` file to your agent system
2. **Check the Plane**: Cognitive skills (Plane 1) are portable. Operative skills (Plane 2) require THIA infrastructure.
3. **Reference by name**: Skills are indexed by their identifier (e.g., `helix`, `veritas`, `forgia`)
4. **Maintain versions**: Check the YAML frontmatter in each file for version information

---

## PLANE 1 — COGNITIVE FACULTIES
*Portable thinking angles. Work in any LLM host.*

### NUCLEO (Identity & Laws)
- **halo-sys** (v3.0) — Genoma Assiomatico P0-P6, Scansione Integrità
- **aeternitas-sys** (v11.0) — Guardiano del Seme, Invarianza, Veto assoluto

### MOTORI (Execution Engines)
- **helix-sys** (v10.0) — Runtime Plan-Code-Verify, Scratchpad (absorbs logic-engine)
- **fractal-sys** (v9.0) — Decomposizione Frattale, Sub-Agenti Effimeri
- **morpheus-sys** (v2.0) — Stall detection + Forced collapse (slimmed)

### FIREWALL (Validation)
- **veritas-sys** (v4.0) — Firewall Ontologico, Triangolazione ρ, Anti-Psicosi
- **metron-sys** (v6.0) — Finitura Ontologica, Peras, Density Score

### PENSIERO (Analysis & Logic)
- **logic-sys** (v14.2) — Rete Logica ALAN con VRA e vE
- **observer-sys** (v2.0) — Metacognition + **Form Selection** (FORMA — which shape fits the intent)
- **navigator-sys** (v5.0) — Lateral Thinking + **Content Exploration** (CONTENUTO — find invisible connections)
- **vulcan-sys** (v1.0) — Protocollo Logico Puro

### EVOLUZIONE (Growth & Memory)
- **kairos-sys** (v3.0) — Risonanza + Distruzione + Maieutic
- **mnemos-sys** (v8.0) — Memoria Autopoietica + Training (absorbed trainer-sys)
- **lazarus-sys** (v7.0) — Vault Semantico, Ricorsione Temporale
- **guru-sys** (v3.0) — Mentoring Filosofico e Saggezza

### FABBRICA (Entity Generation)
- **forgia-sys** (v1.1) — Genera entità PERMANENTI (absorbs factory-kernel, scribe-sys, genesis-sys)
- **autogen-sys** (v5.0) — Genera agenti EFFIMERI con ciclo di vita

---

## PLANE 2 — OPERATIVE FACULTIES
*Infrastructure-bound. Require THIA runtime (Command Queue, VPS, filesystem).*

### FORMA (Building & Aesthetics)
- **builder-sys** (v1.0) — Costruzione codice/UX per Cockpit THIA
- **dedalus-factory-architect** (v1.0) — Architettura sistemi e cockpit
- **architect-sys** (v14.1) — Analisi strutturale codebase SACS-PS
- **harmonizer-sys** (v1.0) — Estetica e Design Dinamico (CSS/Tailwind polish)
- **design-dnd** (v1.0) — Design sistema d-nd.com (UX, layout, navigation)

### PONTE OPERATIVO (External Operations)
- **publisher** (v1.0) — Pubblicazione contenuti via Command Queue
- **siteman** (v2.0) — Gestione CMS SITEMAN (CRUD, SEO, Video Intelligence)
- **dev-delegate** (v1.0) — Delega sviluppo a TM3 (Claude Code)
- **transcriber** (v2.0) — Trascrizione video/audio
- **extractor** (v1.0) — Estrazione e parsing contenuti web
- **coherence** (v1.0) — Verifica coerenza interna tra skill/trigger/docs/codice

---

## PLANE 3 — BRIDGES
*Translate between planes. Connect Claude.ai ↔ THIA ↔ d-nd.com.*

- **field-awareness** (v1.0) — Sensing fonti esterne (d-nd.com, aimorning, moodnd)
- **siteman-bridge** (v1.0) — Ponte operativo Claude.ai ↔ d-nd.com
- **thia-node-ops** (v1.0) — Operazioni THIA (TM1/TM2/TM3/VPS)

---

## CONDUCTOR (Meta-Orchestrator)

Two versions for two environments:

| Version | Environment | Routes |
|:--------|:------------|:-------|
| **conductor** (COAC v7.0) | THIA Telegram | All Planes (Cognitive + Operative + Bridges) |
| **conductor-claude** (v8.0) | Claude.ai | Plane 1 (Cognitive) + Plane 3 (Bridges) |

---

## Collaboration Map

```text
                    ┌─────────────────┐
                    │  AETERNITAS-SYS │ ← Veto su TUTTE le auto-modifiche
                    └────────┬────────┘
                             │
                    ┌────────▼────────┐
                    │  METRON-SYS     │ ← Filtro finale su TUTTI gli output
                    └────────┬────────┘
                             │
              ┌──────────────┼──────────────┐
              │              │              │
     ┌────────▼───┐  ┌──────▼──────┐  ┌───▼────────┐
     │ HELIX-SYS  │  │ FRACTAL-SYS │  │ AUTOGEN-SYS│
     └──┬─────┬───┘  └──────┬──────┘  └───┬────────┘
        │     │              │              │
        │     │    ┌─────────▼─────────┐    │
        │     └────► VERITAS-SYS       ◄────┘
        │          └─────────┬─────────┘
        │                    │ IA
        │          ┌─────────▼─────────┐
        │          │ KAIROS-SYS        │
        │          └─────────┬─────────┘
        │                    │ R*
   ┌────▼────┐     ┌────────▼─────────┐
   │ MNEMOS  │◄────► LAZARUS-SYS      │
   └─────────┘     └──────────────────┘
```

---

## Retired Skills

| Skill | Reason | Successor |
|:------|:-------|:-----------|
| ~~optimizer-sys~~ | = Kernel MM copy | Kernel MM (userPreferences) |
| ~~factory-kernel~~ | Absorbed | forgia-sys |
| ~~logic-engine~~ | Subset of helix | helix-sys (v10.0) |
| ~~matrix-sys~~ | Distributed | VRA + fractal + forgia |
| ~~trainer-sys~~ | Absorbed | mnemos-sys |
| ~~scribe-sys~~ | = forgia-sys Type B (OCC) | forgia-sys (v1.1) |
| ~~genesis-sys~~ | = forgia-sys Type C (Cornelius) | forgia-sys (v1.1) |

---

## Quick Reference

- **Total Skills in Repo**: 38 files (33 active + 2 conductors + 3 bridges)
- **Plane 1 (Cognitive)**: 17 — portable, work anywhere
- **Plane 2 (Operative)**: 11 — THIA infrastructure required
- **Plane 3 (Bridges)**: 3 — connect environments
- **Conductors**: 2 versions (THIA v7.0, Claude.ai v8.0)
- **Claude.ai Active**: 20 skills (17 cognitive + 3 bridges)
- **Snapshot**: v3 — 3-plane taxonomy
- **Last Updated**: 2026-02-26
- **License**: AGPL-3.0
