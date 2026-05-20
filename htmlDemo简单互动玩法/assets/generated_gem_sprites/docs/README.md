# v23 Gem Sprite Direction Batch

Date: 2026-05-20

This batch is a first art-direction pass for the current v23/v24 mainline: stone-body processing / cutting / repair / shaping / clean collection. The old appraisal-flow direction is not the target for these assets.

## Generated Sets

Raw stones, 2 versions each:

- `obsidian_A`, `obsidian_B`
- `fluorite_A`, `fluorite_B`

Finished stones, 2 versions each:

- `pearl_A`, `pearl_B`
- `agate_A`, `agate_B`

v24 direct HTML replacement sets:

- Finished stones: `garnet`, `sunstone`, `catseye`, `jadeite`
- Raw stones: `malachite`, `turquoise`, `hetian`, `shoushan`

## Stage Naming

Raw stone sets use six stages:

- `raw_skin.png`: large rough body wrapped in stone skin
- `cut_inner.png`: smaller complete internal stone after cutting
- `cracked.png`: cut body with visible fine cracks
- `repaired.png`: cracks repaired
- `shaped.png`: shaped gemstone
- `cleaned.png`: final polished clean reward

Finished stone sets use four stages:

- `raw_finished.png`: existing finished stone before work
- `cracked.png`: damaged / cracked state
- `repaired.png`: repaired state
- `cleaned.png`: final polished clean reward

## Folder Layout

- `raw/`: original generated sheets
- `processed/<set>/`: sprite-skill processed sheets, transparent sheet, frames, GIF, and QC metadata
- `stages/<set>/`: handier per-stage PNGs for HTML replacement experiments
- `docs/`: this direction note and prompt summary

## Current QC

The generate2dsprite processor completed for all 16 stored sets. `pipeline-meta.json` reports no edge-touch frames in this pass.

The v24 HTML currently maps all 12 gem ids to `assets/gems_v24`, with the first selected direction for obsidian / fluorite / pearl / agate and direct replacement sheets for the remaining 8 gems.
