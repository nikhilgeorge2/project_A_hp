# Project A — Harry Potter Character Network
## Student Guide · YTS+ DSEB 2026 · Plaksha University

---

## The two questions you are answering

**Q1 — Remove Harry.** Which character is the true leader of each world — and does that match how you read the books?

**Q2 — Refused meetings.** The network predicted these meetings. Rowling refused them. Which one would you write into the movies — and why does the network say it should exist?

Your final presentation answers both questions using data from the network.

---

## Before you open any notebook

Each student writes down independently — no discussion:
1. The 5 characters you believe the story could least afford to lose.
2. Your prediction: if Harry were removed from all 7 books entirely, who becomes the most important character?

**Paper. Sealed. You will open these at the end of the project.**

---

## What you are working with

```
project_A_hp/
  nb1_network_and_degree.ipynb   ← Session 1
  nb2_communities.ipynb          ← Sessions 2–3
  nb3_predictions_and_refusals.ipynb  ← Session 4
  data/
    hp_book1_edges.csv  →  hp_book7_edges.csv
    hp_all_edges.csv
    characters.csv
    common_neighbors_book3.csv
    never_meeting_pairs.csv
    community_analysis.csv
```

Each edge file has three columns: `source`, `target`, `weight`. Weight is co-appearance count within 14 words. This is **not** a friendship network — it records which characters Rowling chose to place in the same moment, whether they are allies or enemies or strangers.

---

## What each notebook asks you to do

### Notebook 1 — The Network and Degree (Session 1)

You will look at the raw data before building anything, then build the Book 3 network and measure weighted degree. You will also track how the network changes across all 7 books.

**At the end of Notebook 1 you will have written:**
- An answer to: what does the distribution of edge weights tell you?
- Your degree predictions — and where they were right or wrong
- A paragraph explaining the network expansion pattern using plot knowledge

---

### Notebook 2 — Community Detection and Removing Harry (Sessions 2–3)

You will explore the pre-computed community data, run Louvain on Books 3, 5, and 7, and then load the pre-computed within-community rankings to answer Q1.

**At the end of Notebook 2 you will have written:**
- Named communities from the algorithm output — Book 3, 5, 7
- Which community surprised you most
- A description of Harry's changing community across books
- Your interpretation of the Slytherin finding (Goyle > Draco)
- Your interpretation of the Order finding (Sirius vs Dumbledore)
- A 4–5 sentence argument on Hermione > Ron — you must take a position

---

### Notebook 3 — Predictions and Refusals (Session 4)

You will explore the common neighbor data, test your predictions, and find the genuine refusals — pairs who share many mutual characters and never share a scene. You will write a screenwriter pitch for one of them.

**At the end of Notebook 3 you will have written:**
- Your pair predictions — and which were right
- An explanation of one prediction failure
- Your reading of the precision curve
- A 60-second screenwriter pitch for one genuine refusal

---

## The presentation (Session 5, June 6)

20 slides. Your team presents. Required structure:

| Slides | Content |
|---|---|
| 1–2 | What the network is and what it measures |
| 3–5 | Network expansion — three Rowling decisions visible in data |
| 6–11 | Q1: Remove Harry — Draco/Goyle, Sirius/Dumbledore, Hermione/Ron |
| 12–17 | Q2: Triadic closure, the refusals, your screenwriter pitch |
| 18–19 | What the network can and cannot see |
| 20 | One sentence: what did you learn that you didn't know from reading? |

Every claim in the presentation must be backed by a number from your notebooks.

---

## What the network can and cannot see

The network measures co-appearance from text. It can see:
- How often Rowling placed two characters in the same moment
- Which characters share the same narrative world
- Which meetings the structure predicts — and which Rowling refused

The network cannot see:
- Dialogue — what characters say to each other
- Emotion — whether a relationship is friendship, rivalry, or love
- Narrative weight — a throwaway mention and a crucial scene look the same
- Time — a meeting in Book 3 and a meeting in Book 7 are treated identically

When your interpretation conflicts with the data, ask: is the algorithm wrong — or did Rowling write one thing and present another?

---

## How to run the notebooks

```bash
# Activate the environment
conda activate clean_env

# Open Jupyter
jupyter notebook
```

Or open each `.ipynb` file directly in VS Code or JupyterLab.

Data loads from `data/` (relative path). No internet required.
