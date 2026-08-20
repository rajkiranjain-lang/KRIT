# READ60 // KRIT

Cinematic, India-first intelligence and reading platform.

## Current status

**Foundation repository initialized.** The current `index.html` is the desktop-first KRIT shell. It intentionally does not load a third-party or generated India map yet.

## Locked product rules

1. **India first:** political and administrative geography must use authoritative Government of India / Survey of India data. No generated or questionable third-party India boundaries.
2. **Verified data:** anything READ60 presents as factual must have a trustworthy, traceable source. AI is an interpretation layer, not the source of truth.
3. **Contextual UI:** location context and actions appear on interaction. Do not permanently cover the map with unnecessary sidebars or menus.
4. **100% working:** features are not considered complete until they actually work with real data. Desktop/laptop/TV is the primary experience; mobile will receive a separate UX strategy later.

## Content principles

- News/info: concise source-based presentation with original-source attribution and link.
- Images: do not copy/re-host without permission; use permitted display/embed mechanisms and attribution.
- Video: play inside READ60 only through an allowed official/embed mechanism; otherwise link to the source.
- Blogs: full-text display only where republication rights/permission permit it; otherwise summary/excerpt plus original link.
- Languages: users may choose English, a local/Indic language, or later an automatic preference. Login remains optional.

## Geographic source

Survey of India is the authoritative source selected for READ60's India political/administrative map layer. The initial target dataset is its **Administrative Boundary Database for the entire country up to district level**, which provides state and district boundaries.

The repository must not replace this with an AI-generated silhouette or an unrelated public GeoJSON.

## Architecture direction

India → State/UT → District → contextual categories → verified content → KRIT assistance.

The map is the primary navigation surface. Backend, ingestion, verification, accounts, analytics, media, and KRIT query services will be added incrementally.
