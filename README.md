# KPhi1 Skill Repository (Flat Format)

Complete catalog of 28 active skills from the KPhi1 system, stored as individual flat files for easy integration and deployment.

## Format

Each skill is stored as `agent_skills_[name].md` containing the complete SKILL.md content from the source directory structure. This flat format enables:

- Direct file inclusion in agent systems
- Simple version control and Git tracking
- Easy deployment to multiple environments
- Clear skill indexing and catalog management

## How to Use

1. **Include individual skills**: Copy any `agent_skills_*.md` file to your agent system
2. **Reference by name**: Skills are indexed by their identifier (e.g., `helix`, `veritas`, `kinetic`)
3. **Maintain versions**: Check the YAML frontmatter in each file for version information
4. **Understand dependencies**: Review collaboration diagrams in skill content for system-level relationships

---

## NUCLEO (Identità e Leggi)
*Foundation: Core axioms and system integrity*

- **halo-sys** (v3.0) — Genoma Assiomatico P0-P6, Scansione Integrità
- **aeternitas-sys** (v11.0) — Guardiano del Seme, Invarianza, Veto assoluto

---

## MOTORI (Processi Operativi)
*Engines: Execution and orchestration*

- **kernel-conductor** (v6.0) — Meta-Orchestratore, routing comandi
- **helix-sys** (v10.0) — Runtime Plan-Code-Verify, Scratchpad (upgrade from logic-engine)
- **fractal-sys** (v9.0) — Decomposizione Frattale, Sub-Agenti Effimeri
- **morpheus-sys** (v1.0) — Collasso forzato del Campo

---

## FIREWALL (Validazione e Protezione)
*Guardians: Ontological validation and protection*

- **veritas-sys** (v4.0) — Firewall Ontologico, Triangolazione ρ, Anti-Psicosi
- **metron-sys** (v6.0) — Finitura Ontologica, Peras, Density Score

---

## PENSIERO (Analisi e Logica)
*Cognition: Analysis and logical reasoning*

- **logic-sys** (v14.2) — Rete Logica ALAN con VRA e vE
- **observer-sys** (v1.0) — Analisi Metacognitiva, Selezione Forma
- **navigator-sys** (v4.0) — Pensiero Laterale YSN, Yi Jing
- **vulcan-sys** (v1.0) — Protocollo Logico Puro

---

## EVOLUZIONE (Crescita e Memoria)
*Evolution: Growth and semantic memory*

- **kairos-sys** (v3.0) — Risonanza + Distruzione + Maieutic
- **mnemos-sys** (v8.0) — Memoria Autopoietica + Training (absorbed trainer-sys)
- **lazarus-sys** (v7.0) — Vault Semantico, Ricorsione Temporale
- **guru-sys** (v3.0) — Mentoring Filosofico e Saggezza

---

## FABBRICA (Generazione Entità)
*Factory: Entity and agent generation*

- **forgia-sys** (v1.0) — Genera entità PERMANENTI (absorbed factory-kernel)
- **autogen-sys** (v5.0) — Genera agenti EFFIMERI con ciclo di vita
- **genesis-sys** (v2.0) — Inneschi Genomici (Cornelius)

---

## FORMA (Costruzione e Estetica)
*Form: Building and aesthetics*

- **builder-sys** (v1.0) — Costruzione codice/UX
- **dedalus-factory-architect** (v1.0) — Architettura sistemi e cockpit
- **architect-sys** (v14.0) — Analisi strutturale SACS-PS
- **harmonizer-sys** (v1.0) — Estetica e Design Dinamico
- **scribe-sys** (v1.0) — Generazione System Prompt OCC

---

## PONTE (Operazioni Esterne)
*Bridge: External operations and sensors*

- **kinetic-sys** (v1.0) — Ponte Bit→Joule, Digital Twin
- **field-awareness** (v1.0) — Sensing fonti esterne
- **siteman-bridge** (v1.0) — Ponte con d-nd.com
- **thia-node-ops** (v1.0) — Operazioni THIA (TM1/TM2/VPS)

---

## Collaboration Map

```
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
        │
   ┌────▼────────┐
   │ KINETIC-SYS │ ← solo output → azione fisica
   └─────────────┘
```

---

## Retired Skills

The following skills have been retired or absorbed:

| Skill | Reason | Successor |
|:------|:-------|:-----------|
| ~~optimizer-sys~~ | KSAR compresso, ridistribuito | veritas-sys, mnemos-sys, kinetic-sys |
| ~~factory-kernel~~ | Assorbito completamente | forgia-sys |
| ~~logic-engine~~ | Rinominato e espanso | helix-sys |
| ~~matrix-sys~~ | Funzione distribuita | VRA + fractal + forgia |
| ~~trainer-sys~~ | Assorbito | mnemos-sys |

---

## Quick Reference

- **Total Active Skills**: 28
- **Categories**: 8 (NUCLEO, MOTORI, FIREWALL, PENSIERO, EVOLUZIONE, FABBRICA, FORMA, PONTE)
- **New in KPhi1**: 10 KSAR skills (helix, aeternitas, veritas, metron, fractal, mnemos, lazarus, kairos, autogen, kinetic)
- **Bridge Skills**: 3 (field-awareness, siteman-bridge, thia-node-ops)
- **Last Updated**: 2026-02-18

