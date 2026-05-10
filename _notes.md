# Revision Notes

Track what you've added, removed, or rewritten here.

---

## 2026-05-05 — Attenborough × Feynman conversion run

Converted all 30 chapters from OpenStax-derived source subfolders into single rewritten markdown files in the **Attenborough × Feynman v1.1** style. Source: 30 subfolders, ~180 OpenStax CNX module files, ~449,718 source words. Output: 30 chapter files + 30 pantry + 30 images briefs + 30 bookmaps = **120 new markdown files**, totaling roughly 157,000 chapter words plus companion materials.

This book has no Part-divider folders — all 30 subfolders had source content.

### Per-chapter results

| # | Chapter | Words | Status | Source folder |
|---|---|---|---|---|
| 01 | science-and-the-universe-a-brief-tour | 5,060 | OK | preserved (see deletion note) |
| 02 | observing-the-sky-the-birth-of-astronomy | 4,320 | OK | preserved |
| 03 | orbits-and-gravity | 6,412 | OK | preserved |
| 04 | earth-moon-and-sky | 3,174 | **FLAGGED — below 3,500 cleanup threshold** | preserved (manual review) |
| 05 | radiation-and-spectra | 7,143 | OK | preserved |
| 06 | astronomical-instruments | 5,750 | OK | preserved |
| 07 | other-worlds-an-introduction-to-the-solar-system | 4,878 | OK | preserved |
| 08 | earth-as-a-planet | 7,241 | OK | preserved |
| 09 | cratered-worlds | 5,455 | OK | preserved |
| 10 | earthlike-planets-venus-and-mars | 5,063 | OK | preserved |
| 11 | the-giant-planets | 6,087 | OK | preserved |
| 12 | rings-moons-and-pluto | 9,525 | OK — agent went above 8,000 target | preserved |
| 13 | comets-and-asteroids-debris-of-the-solar-system | 4,306 | OK | preserved |
| 14 | cosmic-samples-and-the-origin-of-the-solar-system | 5,249 | OK | preserved |
| 15 | the-sun-a-garden-variety-star | 3,651 | OK | preserved |
| 16 | the-sun-a-nuclear-powerhouse | 3,853 | OK | preserved |
| 17 | analyzing-starlight | 4,771 | OK | preserved |
| 18 | the-stars-a-celestial-census | 3,820 | OK | preserved |
| 19 | celestial-distances | 5,044 | OK | preserved |
| 20 | between-the-stars-gas-and-dust-in-space | 3,796 | OK — files were initially written to outputs/, copied to canonical paths | preserved (note: pantry/images/bookmaps were originally named `20-between-the-stars-*` without the full slug; canonical copies in place) |
| 21 | the-birth-of-stars-and-the-discovery-of-planets-outside-the-solar-system | 6,113 | OK | preserved |
| 22 | stars-from-adolescence-to-old-age | 5,521 | OK | preserved |
| 23 | the-death-of-stars | 4,168 | OK | preserved |
| 24 | black-holes-and-curved-spacetime | 5,693 | OK | preserved |
| 25 | the-milky-way-galaxy | 5,611 | OK | preserved |
| 26 | galaxies | 5,249 | OK — files were initially written to outputs/, copied to canonical paths | preserved |
| 27 | active-galaxies-quasars-and-supermassive-black-holes | 4,437 | OK | preserved |
| 28 | the-evolution-and-distribution-of-galaxies | 5,525 | OK | preserved |
| 29 | the-big-bang | 4,405 | OK | preserved |
| 30 | life-in-the-universe | 6,289 | OK | preserved |

**29 of 30 chapters passed the 3,500-word verification threshold.** One chapter (Ch 4 Earth-Moon-and-Sky at 3,174 words) flagged for manual review.

### Companion files generated

For every chapter (30 total): `pantry/NN-slug.md`, `images/NN-slug.md`, `bookmaps/NN-slug.md`.

### Path issues caught and fixed

Two chapters' agents wrote files to `/sessions/brave-admiring-sagan/mnt/outputs/` rather than the canonical book folder. Files copied from outputs/ to the book's `chapters/`, `pantry/`, `images/`, `bookmaps/` folders:

- **Ch 20 between-the-stars-gas-and-dust-in-space** — agent wrote to `outputs/20-between-the-stars-gas-and-dust-in-space.md`, `outputs/20-between-the-stars-pantry.md`, etc. Copied to canonical names with full slug.
- **Ch 26 galaxies** — agent wrote to `outputs/26-galaxies.md`, `outputs/26-galaxies-pantry.md`, etc. Copied to canonical names.

Original output-folder copies remain (sandbox lacks delete permission) — they can be cleaned manually.

### Source folders — deletion note

The conversion workflow specifies that source subfolders should be removed after verification passes. **The bash sandbox does not have delete permission on the mounted folder** — every `rm -rf chapters/NN-slug/` returns "Operation not permitted." All 30 source subfolders remain intact.

**Source folders that passed verification — safe to remove manually:**
01, 02, 03, 05, 06, 07, 08, 09, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30.

**Source folder to PRESERVE pending manual review:**
04-earth-moon-and-sky (chapter at 3,174 words, below 3,500 cleanup threshold; possibly worth expanding using deferred source material logged in bookmap, or accepting the shorter length).

### Combined Test — pass rate

All 30 chapters reported 14/14 Combined Test pass per their conversion agents. The single chapter below threshold (Ch 4) passed all 14 style/content tests but fell short of the 3,500-word cleanup threshold per the workflow's failure-handling rule.

### Notable conversion decisions

- **Heaviest deferrals** in Chs 23 (death of stars, ~22K source words), 28 (galaxy evolution, ~19K), 29 (Big Bang, ~23K), 30 (life in the universe, ~18K), 11 (giant planets had a thin source but the chapter goes deep on metallic hydrogen), 24 (black holes, ~17K). For each, agents picked the strongest 3 scaffolded concepts and logged deferred material to the bookmap.
- **Ch 12 Rings, Moons, and Pluto** went above the 8,000-word target (9,525 words). The agent treated each major moon system as a separate scene, which the source supported richly. Worth Nik's review on whether to trim.
- **Cosmic-scale chapters** (Ch 19 distances, Ch 25 Milky Way, Ch 28 evolution, Ch 29 Big Bang) made heavy use of the workflow's "scale oscillation" rule — moving between intimate (Bessel measuring 61 Cygni; Hubble at Mt Wilson; Penzias and Wilson at Crawford Hill) and cosmic (parsecs, megaparsecs, gigaparsecs).
- **Mechanism-rich chapters** (Ch 5 radiation, Ch 16 nuclear sun, Ch 17 starlight, Ch 23 stellar death, Ch 24 black holes, Ch 29 Big Bang) had the strongest first-principles deep-dives — Planck quantization, proton-proton chain with quantum tunneling, OBAFGKM ionization classification, Chandrasekhar limit from electron degeneracy, Schwarzschild radius derivation, the three pillars of cosmological evidence.
- **OpenStax CNX formatting** (`:::: {#fs-id...}` "Teacher Support" callouts, `<figure>` references, module IDs) was filtered out; substantive content preserved or logged as deferred.

### Next-pass items

- **Source-folder cleanup:** manually remove the 29 verification-passing source subfolders if desired.
- **Review Ch 4** — chapter is below 3,500 threshold. Either expand from deferred source material or accept the shorter length.
- **Review Ch 12** — chapter exceeded the 8,000-word target. Consider whether to trim.
- **outputs/ folder cleanup:** the 8 misplaced files for Chs 20 and 26 still exist in `/sessions/.../mnt/outputs/`. Canonical copies are in place.
- **Review the 30 bookmaps as a set** — deferred-material lists across chapters tell you what astronomy topics need separate study guides or future chapters.
