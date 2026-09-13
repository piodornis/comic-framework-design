# Comic Design Standard v1 - Design Archive Policy

## Contents

- [Purpose](#purpose)
- [Git and archive roles](#git-and-archive-roles)
- [When to archive](#when-to-archive)
- [When not to archive](#when-not-to-archive)
- [SUPERSEDED versus archived](#superseded-versus-archived)
- [Recommended archive layout](#recommended-archive-layout)
- [Archive metadata](#archive-metadata)
- [Large visual artifacts](#large-visual-artifacts)
- [Approval and destructive actions](#approval-and-destructive-actions)
- [Review behavior](#review-behavior)
- [Version](#version)

This document defines how obsolete, replaced, or historically useful visual-development material should be retained in projects compatible with `comic-design-standard-v1`.

## Purpose

Preserve useful design history without allowing old explorations or replaced designs to compete with the current visual source of truth.

Archiving is supplementary. It is not a substitute for clear design states or version control.

## Git and archive roles

Use Git as the primary history for text files and other repository-friendly assets.

Use `design/archive/` when keeping an older visual artifact in the active design folders would create confusion, or when a clearly separated historical copy is useful to creators and reviewers.

Do not create duplicate archive copies merely because Git already contains an older revision.

## When to archive

Archive when one or more of these conditions apply:

- a replaced character or environment design remains creatively or historically useful
- a prior approved design was intentionally replaced
- an exploration set is valuable but should no longer appear among active candidates
- a previous Style Pack version must remain available for comparison or reproduction
- an obsolete source-reference set should be retained for provenance
- moving the material out of active folders materially reduces ambiguity

## When not to archive

Do not archive merely because:

- a routine edit was made
- Git already preserves the required history
- an exploration is still active
- a selected design is still under development
- the creator has not decided whether the material is obsolete

Do not use archiving as a hidden deletion mechanism.

## SUPERSEDED versus archived

`SUPERSEDED` is a design state. `archive/` is a storage location.

They are related but not identical.

A design may be `SUPERSEDED` and remain beside the current design when comparison is useful.

A file may be archived because it is no longer operationally useful even if its historical metadata records another prior state.

When a current design replaces an older one, prefer explicitly marking the older record `SUPERSEDED` before or while archiving it.

Do not treat archived material as current design authority.

## Recommended archive layout

A project may use:

```text
design/archive/
├── characters/
├── environments/
├── props/
├── styles/
├── references/
└── explorations/
```

Create only the subfolders that are actually needed.

Recommended naming pattern:

```text
<subject>__<artifact>__v<version>__<date>.<ext>
```

Example:

```text
b21__character-sheet__v02__2026-09-13.png
maintenance-hall__environment-sheet__v01__2026-09-13.png
```

Use the project's established naming convention when one exists.

## Archive metadata

When practical, record:

- subject or artifact ID
- prior design state
- reason for archival
- replacement artifact, if any
- archive date
- Style Pack and version
- Transformation Profile, if relevant
- important provenance or rights notes

For image-only assets, keep metadata in a nearby Markdown record when embedding metadata is unreliable.

## Large visual artifacts

Large generated images, source photos, layered files, and high-resolution exports may not be suitable for ordinary Git history.

Follow the project's storage policy for large files.

If the project uses Git LFS or external asset storage, record stable references rather than creating uncontrolled duplicate copies.

Do not assume an external storage system unless the project explicitly defines one.

## Approval and destructive actions

Archiving, moving, replacing, or deleting project assets requires explicit creator authorization when it changes the active project structure or removes an artifact from its current location.

Never silently:

- archive a file
- delete a file
- overwrite an approved or locked design
- mark a design `SUPERSEDED`
- change `APPROVED` or `LOCKED` state

A Skill may recommend these actions and explain why.

## Review behavior

Routine design reviews should focus on active design material.

Skip archived material as current authority unless:

- the creator asks for historical comparison
- provenance is relevant
- a regression is being investigated
- an active file explicitly references the archived artifact

If archived material conflicts with current approved or locked material, prefer the current active design and note the historical conflict only when relevant.

## Version

Framework contract: `comic-design-standard-v1`
