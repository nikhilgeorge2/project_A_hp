# Project A — Harry Potter Character Network
## YTS+ DSEB 2026 · Plaksha University

---

## What this project is

You will build and analyse a network of Harry Potter characters, then present what you found as an investigation report.

The network measures co-appearance within 14 words across all 7 books — not friendship, not importance, not dialogue. A throwaway mention and a crucial scene look identical. Everything you find must be interpreted through that constraint.

---

## Getting started

```bash
git clone https://github.com/nikhilgeorge2/project_A_hp.git
cd project_A_hp
jupyter notebook
```

Work through the notebooks in order:

| Notebook | What you do |
|---|---|
| `nb1_network_and_degree.ipynb` | Build the network, measure degree, track expansion across 7 books |
| `nb2_communities.ipynb` | Detect communities, remove Harry, find who leads each world |
| `nb3_predictions_and_refusals.ipynb` | Predict future meetings using common neighbors, find the genuine refusals |

---

## The presentation

**15–20 slides. You choose the structure.**

Before you open any slide software: go back through your notebooks and find the moment where you thought *that's weird* or *I didn't expect that*. That is your presentation.

Every good investigation report has five parts:

1. **The question** — what did you set out to understand?
2. **The instrument** — what does your data measure, and what does it not?
3. **What you found** — three to five findings, each with a number
4. **Where the data surprised you** — the most important part
5. **Your answer** — one sentence, data-backed

---

## Chart rules

Every chart you put in the presentation must follow these:

1. Label every axis — name and unit
2. No index numbers on axes — 0, 1, 2, 3 from your dataframe carry no information; replace them with actual names or values
3. Title states the finding, not the variables — not *"Degree vs betweenness"* but *"Two measures, two different answers"*
4. One chart, one claim
5. Don't put it in if you can't explain every element — you will be asked
6. Label the interesting point directly — annotate it, circle it
7. If you use ranks, say which direction is better — write *(1 = highest)* on the chart
8. Remove decoration that carries no information — no 3D bars, no background gradients
9. Consistent colours — if Hermione is purple in one chart, she is purple in every chart
10. Every number on the chart comes out of your mouth — if you skip over it while presenting, it shouldn't be there

---

## Image policy

- Charts you generated: always fine
- HP movie stills, book covers, character art: **do not use** — copyrighted (Warner Bros. / Bloomsbury)
- Wikipedia images: fine, include the URL below the image
- Your charts are your visuals — every slide that makes a claim should show the chart that backs it

---

## Data citation

> Ravi, N. (n.d.). *Harry Potter character interaction network* [Dataset]. GitHub.
> https://github.com/nikhil-ravi/harry-potter-interactions

Cite this on the slide where you introduce the network.
