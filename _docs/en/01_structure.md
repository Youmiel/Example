# Structure

## Definition

- `category`: a set of contraptions that share similar features (e.g. "Mob Resources", "Block Resources", "SlimeStone")
- `contraption`: a set of design for a common purpose (e.g. "Cobblestone Generator", "Univeral Tree Farm")
- `design`: a specific design from player(s), ususally contains a description and one or more works (e.g. world save, schematic, etc.)

## Details

The repository is structured as follows:

- `_docs/`: documentation files
- `_knowledge/`: knowledge base files
- `_example-category/`: example

- `<category1>/`
  - `<contraption1>/`
    - `<design1>/`
    - `<design2>/`
    - ...
  - `<contraption2>/`
  - ...
- `<category2>/`
  - ...
- `<category3>/`
  - ...
- ...

For each design in the contraption folders, the structure is as follows:

- `<unique id to the design>/`: a unique identifier for each design
  - `description.md`: description of the design, can be written in any language
  - `media/`: media files used in the description
  - `works/`: contains world saves, schematics, or other formats of the design
  - `metadata.json`: metadata for programs (e.g. "Author Names", "Release Dates", "License")

**Design id format**: `[date]__[design-name]`, `[date]` is the release date in `YYYY-MM-DD` format, and `[design-name]` is a short, hyphen-separated name (e.g., `2025-06-08__72K-Ghost-Block-Farm`). Author names are not included in the id to avoid complications with special characters and multiple authors.
