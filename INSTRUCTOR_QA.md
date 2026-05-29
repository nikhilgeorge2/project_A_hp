# Project A — Harry Potter Network
## Instructor Q&A Reference · YTS+ DSEB 2026

25 questions students will encounter or should be able to answer. Answers marked **[student]** vary by team.

---

### Part 1 — The Network and What It Measures

**1. What does an edge in this network represent?**
Two characters appearing within 14 words of each other in the text — co-mention, not dialogue, friendship, or interaction.

**2. What does edge weight measure?**
How many times that co-appearance happened across the book — frequency of proximity, not strength of relationship.

**3. Why does the network shrink from Book 1 (122 nodes) to Book 3 (90 nodes)?**
Rowling tightened the world — Books 2 and 3 are intimate, Hogwarts-focused, few new characters introduced.

**4. Why does the network explode in Book 4 (178 nodes)?**
The Triwizard Tournament brings in students and staff from two other schools — the largest single-book cast expansion.

**5. Why does the network peak in Book 5 (223 nodes)?**
The Order of the Phoenix introduces a large adult cast; Umbridge's regime adds Ministry characters; the DA adds many student names.

**6. Why does the 14-word window undercount intimate scenes between main characters?**
Rowling uses pronouns ("he said," "she replied") in close two-character scenes — no names means no edge counted; minor characters are always named to avoid confusion, so they get overcounted.

---

### Part 2 — Community Detection

**7. What does Louvain community detection do?**
Groups characters who appear together more than they appear with outsiders — using only edge weights, no character names or plot knowledge.

**8. What community does Louvain find in Book 3 that surprises most readers?**
The Marauder community: Sirius, Lupin, Snape, and Pettigrew grouped together — the algorithm found the secret history of Book 3 from scene construction alone.

**9. Why is the Marauder finding surprising?**
These characters are enemies in the plot; the algorithm has no plot knowledge and still groups them because Rowling constructed their scenes together.

**10. Which community is Harry in during Book 5 — the same as Ron and Hermione?**
No. Harry separates into the Order/war world community; Ron and Hermione stay in the school world community.

**11. Where are Snape and Dumbledore in Book 7's community structure?**
In the flashback community — not the Horcrux hunt. The algorithm sorted them by memory, not by the present-tense war.

**12. Which community do Luna and Tom Riddle share in Book 7?**
The Malfoy Manor world — both are drawn into those scenes regardless of their opposing roles in the story.

---

### Part 3 — Remove Harry

**13. Without Harry, who leads the Slytherin world in Book 3?**
Goyle is #1 by within-community degree, Crabbe #2, Draco #3.

**14. Why might this result be an artifact rather than a finding?**
Draco becomes "he" in scenes with Harry (intimate, pronoun-heavy); Goyle is always named as a minor character. The algorithm counted names, not leadership.

**15. Without Harry, who leads the Order world in Book 5?**
Sirius Black is #1 — embedded in the Order community. Dumbledore is #2 across multiple communities but #1 in none (connector, not pillar).

**16. How does Hermione rank vs Ron across Books 3, 5, and 7?**
Hermione is #1, Ron is #2 within the trio community — every single book without exception.

**17. Is the Hermione > Ron finding right or wrong?** **[student]**
Either: the algorithm correctly finds Hermione as structural glue of the trio; or: it misses Ron's emotional/warmth role which doesn't show up in scene proximity counts.

---

### Part 4 — Predictions and Refusals

**18. What is a common neighbor?**
A character connected to both members of a pair — they share mutual acquaintances, which means they inhabit the same narrative world.

**19. What does CN > 10 after Book 3 predict?**
92% chance the pair will share a scene before Book 7 ends — the algorithm predicts meetings from structure alone.

**20. What is a genuine refusal?**
A pair with high CN where both characters are alive, still in the story, and Rowling never put them in the same scene — a deliberate authorial choice.

**21. What is the CN score for McGonagall and Cho Chang, and why do they never meet?**
CN = 40. Both are deeply embedded in Hogwarts — McGonagall is institutional authority, Cho is teenage grief and romance. Rowling maintained the boundary between those two worlds.

**22. Why does a crowd sentence inflate CN scores?**
"Seamus, Dean, Neville, and Lavender all cheered" creates an edge between every pair — the algorithm treats crowd listing as mutual connection, even if the characters have no actual relationship.

---

### Part 5 — Methods and Limitations

**23. What does weighted degree measure and what does it miss?**
Total co-appearances across all partners — how broadly Rowling placed a character across scenes. Misses: who speaks, who leads, emotional weight, and intimate scenes written in pronouns.

**24. Why was betweenness centrality not used in this project?**
The project deliberately excludes it — degree and community detection are sufficient for the two big questions, and betweenness is taught separately. (If a student asks: betweenness would measure which characters connect different factions, which is a different question from who leads each world.)

**25. What is the one-sentence takeaway from this project?** **[student]**
Strong answers will name a specific number and explain the gap between what the algorithm found and what readers remember — e.g.: "The algorithm found that Goyle holds the Slytherin world together (within-rank #1) while readers remember Draco — because the algorithm counted scenes, not narrative agency."
