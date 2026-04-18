# Desert Dev Lab 2026

Resources for the Desert Dev Lab Hackathon 2026.

This repo is organized around **datasets first**. The main goal is to help teams quickly find usable Food & Agriculture data sources, understand what each source contains, and see how it can be used in an app.

## Start Here

- [Dataset index](data-sources/README.md)
- [Food access and affordability datasets](data-sources/food-access/README.md)
- [Growers, land, water, and supply chain datasets](data-sources/growers-and-supply/README.md)
- [Water and climate datasets](data-sources/water-and-climate/README.md)
- [Markets, civic spaces, and local government datasets](data-sources/markets-and-civic-spaces/README.md)
- [Operations, food rescue, and permitting datasets](data-sources/operations-and-recovery/README.md)

## Featured Project Ideas

These are featured example directions for teams that want a starting point. They are meant to spark ideas, not limit what a team can build.

- **Local food resilience:** Albuquerque depends heavily on out-of-state food and processing.
- **New growers:** Upfront land, infrastructure, and startup barriers limit entry.
- **Experienced growers:** Aging producers and succession risk threaten long-term continuity.
- **Community food spaces:** Residents need better ways to shape food-related public spaces over time.

## How To Use This Repo

1. Start with the dataset guide that best matches your idea.
2. Pick 1-3 sources that are realistic for a weekend prototype.
3. Prefer cleaned CSV/JSON inputs over live GIS integrations unless mapping is central to your project.
4. Use the example project ideas as inspiration, not as constraints. Combining datasets across themes is encouraged.

## Repo Structure

```text
README.md
data-sources/
  README.md
  food-access/README.md
  growers-and-supply/README.md
  water-and-climate/README.md
  markets-and-civic-spaces/README.md
  operations-and-recovery/README.md
```

## Notes

- Many of the strongest Albuquerque and New Mexico sources are GIS-based and may need light cleanup before use in a web app.
- Some APIs require keys or tokens. Each dataset guide calls that out explicitly.
- Local freshness can vary, especially for civic layers and operational directories, so teams should spot-check important records before demoing.

## Food & Agriculture Problem Statements

These problem statements have been developed and validated by Subject Matter Experts (SMEs) from the **City of Albuquerque**. Our goal is to provide local builders and developers with a clear direction and real-world insights to help drive impactful projects in the food and agriculture sector. Builders do not have to use these problem statements and are welcome to come up with their own.

### Validated Problem Statements Contributors
The following SMEs provided a variety of food & ag problem statements, based on their expertise and community feedback. Four options of the set are provided below, by:
* Ann Simon (Sustainability)
* Alice Main (Sustainability)
* Sandra West (Sustainability)
* Albert Lee (Sustainability)
* Veronica Blount (Sustainability)
* Solange Archer (Sustainability)
* Jacky So (APINH Affairs, OEI, FUSE)

Relevant public datasets have been compiled based on these problem statements. Jacky So contributed the Food Access dataset with Travis Neufeld contributing all others.

It is encouraged to seek out mentor guidance on problem statement direction and product build.
---

### Problem Statements Table

| Sub-Topic | Problem Statement | Primary Affected Users | Why This Matters | Partner Feedback |
| :--- | :--- | :--- | :--- | :--- |
| Food Access & Affordability | 98% of all food consumed in Albuquerque comes from out of state, indicating an overreliance on the global supply chain and out-of-state processing for food. | Food distributors: Grocery stores, Consessions, Restaurants, etc. | This situation makes it difficult for new, local producers to compete with high-volume, out-of-state prices. It makes our food system more vulnerable to out-of-state supply chain dynamics and reduces our local spending multiplier effect. | [Richmond Fed: Local Spending Multiplier Effect](https://www.richmondfed.org/publications/research/economic_brief/2025/eb_25-28) |
| Local Production & New Growers | New growers lack upfront capital and land access to begin opperations, further exasterbated by urban sprawl and desertification. | New producers | | |
| Local Production & Experienced Growers | Farming and ranching are experiencing an aging and declining workforce. The average age of farmers in New Mexico is greater than most other states. Succession planning ideas are necessary to assure continuation of these industries. | Experienced producers, new producers | | [AI helps John Deere transform agriculture \| OpenAI](https://openai.com/index/john-deere-justin-rose/)<br>[Agriculture Technology \| Precision Ag \| John Deere](https://www.deere.com/en/technology-products/precision-ag-technology/)<br>[Jahmy Hindman on John Deere A.I. Transforming Farming and Yields \| Observer](https://observer.com/2025/09/jahmy-hindman-john-deere-ai-farming/) |
| Markets & Community Spaces | Community members lack consistent ways to influence how food-related public spaces are designed, named, and evaluated over time. | Neighborhood residents, Community organizations | Weak feedback loops can erode trust and long-term engagement. | Qualitative signal; validate strength with partners |