# Presentation Guide — Harry Potter Network
## YTS+ DSEB 2026 · Plaksha University

---

## A suggested spine

This is a starting point, not a template. You found your own interesting things — decide where they live.

| # | Slide |
|---|---|
| 1 | Cover — team, project, date |
| 2 | Why analyse a book as a network? |
| 3 | The data — 7 books, 204 characters, what an edge means |
| 4 | What the network looks like |
| 5 | The simplest question: who appears most? |
| 6 | The answer — and whether it surprises you |
| 7 | A deeper question needs a new concept: groups that stay together |
| 8 | The communities of Book 5 |
| 9 | Now remove Harry |
| 10 | Slytherin: Goyle above Draco |
| 11 | The Order: Sirius leads, Dumbledore spans everything |
| 12 | The trio: Hermione, every time |
| 13 | What the network can and cannot see |
| 14 | A second question: who should have met? |
| 15 | The logic of common neighbors — and it works: 92% |
| 16 | The genuine refusals: high connection, never a scene |
| 17 | The pair we chose |
| 18 | The scene we would write |
| 19 | What this tool cannot see |
| 20 | What we still don't know |

Found something the notebooks didn't ask for? Put it in. Something here doesn't apply? Cut it.

---

## Presenting to someone who has never seen a network

Your audience knows Harry Potter. They do not know what community detection is.

**Introduce each concept at the moment you need it — not before.**
Don't open with a glossary. When you need community detection, explain it in one sentence using HP, then immediately show what it found. The concept earns its place by doing something surprising right away.

**Show it first, name it second.**
Don't say "community detection is an algorithm that groups nodes." Show the Book 5 communities on screen. Let the audience recognise the groups. Then name what the algorithm did. The name lands as recognition, not vocabulary.

**Say what question the concept answers before explaining the concept.**
Before common neighbors: *"We wanted to know which characters should have met, based on who they both knew. Here's how we measured that."*

---

## Telling the story

**Slide 2 should set up an expectation the analysis will then complicate.**
Give the audience something they already believe. Spend the rest of the presentation testing it against the data.

**Each finding should make the next one feel necessary.**
Not: finding 1, finding 2, finding 3.
But: *"Removing Harry changes who leads each world — which made us ask: are there characters the network expected to meet, but never did?"*

**The last slide is not a summary.**
It is the question your data raised but couldn't answer.

---

## Before you finalise any slide

**Showing how something works is not the same as saying what it means.**
"Goyle ranks #1 in the Slytherin community" is a result. "The network sees scene-presence, not narrative agency — which is why both Goyle and Draco might be right" is an interpretation. Both must appear on the same slide.

**Each of the three remove-Harry findings needs to say why it is not just the previous one.**
Goyle, Sirius, Hermione are three different communities with three different puzzles. Open each one with what makes this case distinct — not just "here is another community."

**Read just your slide titles. Does the story make sense?**
Before presenting, read the titles alone, in order. They should tell the investigation. If the story is only clear when you add your voice, the titles are doing too little.

**Your slide title should say exactly what the slide claims — not bolder, not softer.**
"Goyle leads Slytherin" is bolder than what the data shows. "Within-community rank: Goyle above Draco" is accurate. Overclaiming in a title is the most common error.

**Explain every term the first time it appears — in one sentence, inline.**
Not a separate slide. Not a glossary. One parenthetical on first use: *"betweenness centrality (the fraction of shortest paths that pass through a character)."*

---

## Chart rules

1. Label every axis — name and unit
2. No index numbers on axes — replace 0, 1, 2, 3 with actual names or values
3. Title states the finding, not the variables
4. One chart, one claim
5. Don't put it in if you can't explain every element — you will be asked
6. Label the interesting point directly on the chart
7. If you use ranks, say which direction is better — write *(1 = highest)*
8. Remove decoration that carries no information
9. Consistent colours across all slides
10. Every number visible on the chart comes out of your mouth

---

## Images

- Charts you generated: always fine
- HP movie stills, book covers, character art: fine — thanks, Warner Bros.
- Wikipedia images: fine, include the URL below the image
- Your charts are the visuals — not the fandom

---

## Citation

> Ravi, N. (n.d.). *Harry Potter character interaction network* [Dataset]. GitHub.
> https://github.com/nikhil-ravi/harry-potter-interactions

Put this on the slide where you introduce the data.
