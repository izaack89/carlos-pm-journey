# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this vault is

This is **carlos-pm-journey** — an **Obsidian knowledge vault** covering Carlos's
project-management certification journey. Located at
`~/Documents/Personal-Projects/carlos-pm-journey` (moved from
`.../agile/final_project/agil_expansion_lte` in jul-2026). It contains no
executable code — the "build" is opening the vault in Obsidian.

**Each certification lives in its own numbered top-level section with an
identical internal layout.** Current sections:

1. **`01-APL/` — Agile Project Leader** — ✅ COMPLETED. Course (13 modules,
   358 PDFs + 358 notes) + the PIDA project (Telemóvil Costa Rica, 23 sitios
   LTE B41) with all 12 weeks of deliverables.
2. **`02-PMP/` — Project Management Professional** — 📖 IN PROGRESS. Modules 1
   (Gestión del Tiempo y Recursos, 50 files) and 2 (Gestion del alcance, 32 files)
   received, both with study notes + MOC; module 2 also has a quiz bank note.

## Vault structure

```
/
├── Index.md                    ← HOME: dashboard de certificaciones + cómo agregar una nueva
├── 01-APL/
│   ├── Index-APL.md            ← índice del curso APL (13 módulos, links a notes/)
│   ├── documentation/          ← 358 PDFs en 13 carpetas "NN. Nombre"
│   ├── notes/                  ← 358 notas .md espejo de documentation/
│   └── specs/                  ← proyecto PIDA APL (notas de diseño + README)
│       └── entregables/        ← oficiales + semana-1..12 + historico/ + docs vivos
├── 02-PMP/
│   ├── Index-PMP.md            ← índice del curso PMP
│   ├── documentation/
│   │   ├── 01. Gestión del Tiempo y Recursos/   (48 PDFs + 2 mp4)
│   │   └── 02. Gestion del alcance/             (32 PDFs)
│   ├── notes/
│   │   ├── 01. Gestión del Tiempo y Recursos/   (L1-L6 + MOC)
│   │   └── 02. Gestion del alcance/             (L2-L6 + MOC + Quiz + Ideas)
│   └── specs/entregables/      ← para el futuro proyecto aplicado del PMP
├── 99-Templates/
│   └── Template-Certificacion.md   ← plantilla para la certificación N
└── .obsidian/                  ← config (do not edit manually)
```

### Standard layout per certification (`NN-SIGLA/`)

- `Index-SIGLA.md` — course index: modules table, per-module file links,
  trazabilidad with previous certs.
- `documentation/NN. <Módulo>/` — official PDFs/videos as delivered.
- `notes/NN. <Módulo>/` — study notes: one `L<N> - <Título>.md` per lesson +
  one `00-MOC-<Tema>.md` map of content.
- `specs/` — applied project; `specs/entregables/` follows the deliverables
  conventions below.

### Adding a new certification

1. `mkdir NN-SIGLA/{documentation,notes,specs/entregables}` (next number).
2. Copy `99-Templates/Template-Certificacion.md` → `NN-SIGLA/Index-SIGLA.md`, fill it.
3. Add the row to the table in `Index.md` (Home).
4. Add the section to this CLAUDE.md.

### Adding a new module to a certification

Copy the folder to `NN-SIGLA/documentation/NN. <Nombre>/`, add its section to
`Index-SIGLA.md`, and create study notes in `notes/NN. <Nombre>/`.

## Deliverables

Every deliverable produced for an applied project (actas, reportes, dashboards,
bitácoras, DoD, etc.) must be created inside that certification's
**`specs/entregables/`**. Do not scatter deliverable files elsewhere.

### Folder convention inside `entregables/`

- **Week-scoped deliverables** → `semana-N/` (one folder per project week).
- **Project-wide artifacts** (definición, plan de trabajo, defensa, diagramas)
  → `entregables/` root.
- **Superseded versions** → `entregables/historico/`. Never overwrite live
  Delivery files; move the older copy first.

### Deliverable file formats

**`.xlsx`** (spreadsheets with charts/formulas), **`.docx`** (reports, actas),
**`.pdf`** (final exports). Do **NOT** use `.csv` for final deliverables — CSV
carries no charts/formatting; acceptable only as intermediate data.

## Authoring conventions

- **Links to PDFs**: Obsidian wiki-link with explicit path and display name:
  `[[documentation/04. Lean & Kanban/Reglas de tablero Kanban.pdf|Reglas de tablero Kanban]]`
  (path-suffix links resolve regardless of the `NN-SIGLA/` prefix).
- **Internal section links**: `[[#Section]]` same-file; `[[Note#Section]]` cross-note.
- **Language**: content is primarily Spanish; module names may mix Spanish/English.
- **Study note frontmatter**: `title, curso, modulo, leccion, fuente, status
  (por-estudiar/estudiado), tags`.

## APL project facts (authoritative — do not re-litigate)

The APL/PIDA project is COMPLETE. Authoritative artifacts:
`01-APL/specs/entregables/02.DefinicionPIDA...Delivery.docx` and
`03.PlanTrabajo...Delivery.xlsx` (SUBMITTED — do not edit).

- Cliente: **Telemóvil Costa Rica** (NOT Liberty Panamá — early-draft error, corrected).
- Proyecto: 23 sitios LTE banda 41 · Golden Cluster = **3 sitios + 20 restantes**.
- Cronograma: inicio 3-jun-2026 · 8 semanas ejecución + 4 APL · deadlines duros:
  1-jul (Entrega de avance) y 11-ago (Reporte PIDA) · coaching W6 · retros W3/W5/W7/W9.
- Metas: FTR ≥90% (baseline 82-88%) · re-trabajo −10% · DoR ≥85% · bloqueos <72h ≥80%.
- Estado real corte 30-jun (W4): 7/23 aceptados, FTR 96% (CR-001 único FTR=No,
  IMP-02), re-trabajo −11.9%, 1ª retro 17-jun. Aceptación cerró en W9 por desfase
  estructural integración→aceptación.
- Equipo: 3 integradores per Delivery / 4 en el vault (Diego, Ana, Sandeep, Hugo) —
  discrepancia aceptada, no sincronizar a la baja. 3 optimizadores (Marco, Sofía,
  Patricia) · Eduardo (Implementation Manager, peer) · 3 cuadrillas (Luis, Javier, Ricardo).
- Cliente 5 áreas: RAN (Roberto) · Planning (Marcela) · Quality (Patricia) ·
  O&M (Fernando) · Acceptance (Ricardo Mendoza) — nombres placeholder sintéticos.
- Contexto CR: regulador SUTEL · eléctrico ICE/CNFL · site IDs `CR-XXX` con zonas
  🔶 placeholder hasta confirmación.
- Documentos VIVOS de Carlos (no regenerar): `2 Seguimiento_...xlsx`,
  `3.1 Retrospectivas.xlsx`, `Retrabajo técnico.xlsx` (entregables raíz),
  `1.4 Bitacora...FTR.xlsx` (semana-1/). Su convención de nombres usa prefijo de
  actividad del plan (1.1, 1.3, 1.4, 2, 3.1).

## Important quirks

- Folder names with trailing whitespace/punctuation must be preserved exactly
  (in `01-APL/documentation/`): `06. Continuous improvement ` (trailing space),
  `08. Alineación Estratégica en Proyectos.` (trailing dot),
  `11. Liderazgo colaborativo ` (trailing space).
- `02. Detección y Resolución de Riesgos y Problemas copy` — "copy" is canonical.
- Some PDFs exist in accented AND unaccented variants (`Pruebate` vs `Pruébate`) — distinct files.
- macOS stores filenames NFD-decomposed; wiki-links may be NFC. Obsidian resolves
  them fine — when auditing links with scripts, normalize with NFC first.
- `01-APL/Index-APL.md` has ~64 links to notes that never existed in the original
  export (mostly `APL_SC*_R*` resource files) — known pre-existing gaps, not
  caused by any reorganization. Do not "fix" by deleting the links; they document
  which course resources were never converted to notes.
- The vault was renamed/moved in jul-2026: `agil_expansion_lte` →
  `carlos-pm-journey`, then moved up to `Personal-Projects/`. Claude memory was
  migrated each time.

## Git

The vault is a git repo pushed to **private GitHub repo izaack89/carlos-pm-journey**
(created ago-2026). `documentation/` folders (~1.6GB of course PDFs/videos, some
files >100MB) are gitignored — only notes, specs, entregables, templates and
Obsidian config are versioned. After significant vault changes, commit and push.

## Obsidian settings (`.obsidian/`)

Enabled core plugins: file-explorer, global-search, switcher, graph, backlink, canvas, tag-pane, properties, page-preview, daily-notes, templates, outline, bookmarks, bases, sync, file-recovery, word-count.
