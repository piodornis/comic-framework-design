# comic-design-framework

A reusable framework for AI-assisted visual development of comics.

The framework defines how to develop, review, and document visual styles, character designs, environments, props, and reference-driven transformations without embedding the canon or visual identity of a single comic project into reusable Skills.

## Purpose

`comic-design-framework` complements `comic-story-framework`.

- `comic-story-framework` defines narrative truth, characters, relationships, world logic, story, scripts, and storyboards.
- `comic-design-framework` defines how those narrative elements are visually interpreted and approved.
- a future `comic-production-framework` may turn approved story and design material into production-ready panels, pages, lettering, and exports.

The comic project repository remains the source of truth for project-specific content.

## Core model

The framework separates three concepts:

1. **Canon state** — whether a statement is established, inferred, proposed, conflicting, or open.
2. **Design state** — whether a visual solution is exploratory, selected, approved, locked, or superseded.
3. **Visual treatment** — split into reusable **Style Packs** and reusable **Transformation Profiles**.

Example:

```text
photo
  │
  ├── transformation-profile: photo-to-comic
  │
  └── style-pack: franco-belgian-vivid
          │
          ▼
     comic design exploration
```

The transformation profile controls what to preserve or reinterpret from the source material. The style pack controls the visual language.

## Framework contract

The design schemas in this repository define `comic-design-standard-v1`.

They are intended to work alongside `comic-project-standard-v1` from the story framework. The design framework must not silently change narrative canon. New narrative facts discovered or invented during design work remain `PROPOSAL`, `INFERENCE`, `CONFLICT`, or `OPEN` until explicitly accepted.

## Repository structure

```text
comic-design-framework/
├── README.md
├── skills/
│   ├── comic-style-director/
│   ├── comic-character-designer/
│   ├── comic-environment-designer/ (planned)
│   └── comic-design-reviewer/ (planned)
├── schemas/
│   ├── design-status.md
│   ├── visual-style-schema.md
│   ├── style-pack-schema.md
│   ├── transformation-profile-schema.md
│   ├── character-design-schema.md
│   ├── environment-design-schema.md
│   ├── visual-reference-schema.md
│   └── design-review-schema.md
├── style-packs/
│   └── franco-belgian-vivid/
│       └── style.md
├── transformation-profiles/
│   └── photo-to-comic/
│       └── transformation.md
└── templates/
    └── comic-project-design/
        ├── design-project.md
        └── design/
            ├── styles/
            ├── characters/
            ├── environments/
            ├── props/
            ├── references/
            └── archive/
```

## v1 Skills

Current and planned Skill set:

- `comic-style-director` — implemented; define, select, compare, evolve, and visually explore visual styles and Style Packs.
- `comic-character-designer` — implemented; develop new character designs or refine existing drafts, character sheets, turnarounds, variants, expressions, costumes, equipment, continuity anchors, and visual identity.
- `comic-environment-designer` — planned; develop locations, architecture, environments, props, machinery, and related visual world elements.
- `comic-design-reviewer` — planned; review visual consistency, style compliance, source fidelity, repeatability, and approval readiness.

In v1, props, vehicles, costumes, creatures, and related design objects remain responsibilities of the character or environment designer unless repeated real-world use shows that a dedicated Skill is needed.

## Reusable versus project-specific styles

Reusable visual languages may live in this framework as Style Packs.

Example:

```text
style-packs/franco-belgian-vivid/
```

A project-specific identity should normally live inside the comic project itself.

Example:

```text
human-park/
└── design/
    └── styles/
        └── human-park/
            ├── style.md
            └── references/
```

This prevents reusable Skills from depending on one comic's identity.

## Style Packs and Transformation Profiles

A **Style Pack** answers:

> What should the visual result look and feel like?

A **Transformation Profile** answers:

> When starting from existing source material, what must be preserved, what may change, and what should be transformed?

This separation allows combinations such as:

```text
photo-to-comic + franco-belgian-vivid
photo-to-comic + manga-clean
photo-to-comic + future-style
```

without duplicating the source-preservation workflow for every visual style.

## Project design layer

A compatible comic project may add:

```text
comic-project/
└── design/
    ├── styles/
    ├── characters/
    ├── environments/
    ├── props/
    ├── references/
    └── archive/
```

Use `templates/comic-project-design/design-project.md` as the design-layer entry point.

## Source-of-truth principle

Narrative canon belongs to the comic project. Approved visual solutions also belong to the comic project.

Framework files define reusable process and schema only.

Do not silently copy project-specific designs into reusable Style Packs.

## Version

Framework contract: `comic-design-standard-v1`
