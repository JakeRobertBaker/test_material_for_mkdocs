# CLAUDE.md

## Extensions

This project uses `pymdownx.blocks.admonition` and `pymdownx.blocks.details` (the blocks replacements), not the classic `admonition` / `pymdownx.details`. These must not be mixed with their classic counterparts — the output is identical HTML and they conflict.

## Custom Admonition Types

Custom types require **two** independent layers:

1. **YAML config** (`mkdocs.yml` → `types` list) — registers the name so the parser accepts `/// typename`. Without this, the block syntax is rejected.
2. **CSS** (`docs/stylesheets/extra.css`) — styles the resulting `.admonition.typename` class. Without this, the type renders with the default `note` fallback colours.

Neither layer replaces the other.

## Colour Reference

Material's built-in admonition colours are defined in `~/mkdocs-material/src/templates/assets/stylesheets/main/extensions/markdown/_admonition.scss` (lines 31–44). The custom types in this project map to:

| Custom Type  | Matches  | Hex       |
|-------------|----------|-----------|
| definition  | note     | `#448aff` |
| proposition | tip      | `#00bfa5` |
| lemma       | success  | `#00c853` |
| theorem     | question | `#64dd17` |
| proof       | quote    | `#9e9e9e` |

## Cross-Referencing

Blocks support `attrs: {id: anchor-name}` in YAML options to set an ID on the container div. Reference with `[text](#anchor-name)` on the same page or `[text](./other.md#anchor-name){data-preview}` across pages. Requires `attr_list` extension.

## Material Type Registration

Material for MkDocs defines 12 admonition types (note, abstract, info, tip, success, question, warning, failure, danger, bug, example, quote). The pymdownx.blocks.admonition defaults are different (note, attention, caution, danger, error, tip, hint, warning, important). All 12 Material types must be explicitly listed in the `types` config in `mkdocs.yml` or they won't be recognised by the blocks parser.
