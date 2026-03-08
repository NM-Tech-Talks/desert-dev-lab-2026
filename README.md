# Desert Dev Lab 2026

Resources for the Desert Dev Lab Hackathon 2026.

This repo is organized around **datasets first**. The problem statements from the working sheet are still here, but the main goal of the repo is to help teams quickly find usable Food & Agriculture data sources, understand what each source contains, and see how it can be used in an app.

Source problem list: [Food & Ag review sheet](https://docs.google.com/spreadsheets/d/1EN2ns9BAI97obRXzsCTIX5tEi8aBhEP8/edit?usp=sharing&ouid=102887163016251251248&rtpof=true&sd=true)

## Start Here

- [Dataset index](data-sources/README.md)
- [Food access and affordability datasets](data-sources/food-access/README.md)
- [Growers, land, water, and supply chain datasets](data-sources/growers-and-supply/README.md)
- [Markets, civic spaces, and local government datasets](data-sources/markets-and-civic-spaces/README.md)
- [Operations, food rescue, and permitting datasets](data-sources/operations-and-recovery/README.md)

## Featured Hackathon Prompts

The `Go` rows from the sheet are still the featured prompts, but their supporting datasets now live in the guides above.

- **Local food resilience:** Albuquerque depends heavily on out-of-state food and processing.
- **New growers:** Upfront land, infrastructure, and startup barriers limit entry.
- **Experienced growers:** Aging producers and succession risk threaten long-term continuity.
- **Community food spaces:** Residents need better ways to shape food-related public spaces over time.

## How To Use This Repo

1. Start with the dataset guide that best matches your idea.
2. Pick 1-3 sources that are realistic for a weekend prototype.
3. Prefer cleaned CSV/JSON inputs over live GIS integrations unless mapping is central to your project.
4. Use the problem statements as context, not as constraints. Combining datasets across themes is encouraged.

## Repo Structure

```text
README.md
data-sources/
  README.md
  food-access/README.md
  growers-and-supply/README.md
  markets-and-civic-spaces/README.md
  operations-and-recovery/README.md
```

## Notes

- Many of the strongest Albuquerque and New Mexico sources are GIS-based and may need light cleanup before use in a web app.
- Some APIs require keys or tokens. Each dataset guide calls that out explicitly.
- Local freshness can vary, especially for civic layers and operational directories, so teams should spot-check important records before demoing.
