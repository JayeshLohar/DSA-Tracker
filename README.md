# DSA Prep Tracker
 
A single-file, offline checklist for tracking Data Structures & Algorithms preparation for FAANG-level interviews and competitive programming (Codeforces 1500 → 2000+).
 
Open the HTML file in a browser, tick topics as you master them, and watch your rank climb from **Newbie** to **Grandmaster**.
 
---
 
## Features
 
- **383 topics across 22 sections**: arrays, strings, linked lists, trees, graphs, DP, greedy, bit manipulation, number theory, geometry, range-query structures and more
- **Gap sections**: interview-critical patterns, Codeforces-specific techniques and advanced 2000+ topics not covered in most standard checklists
- **Priority tags** (P0 / P1 / P2) to focus on what matters first
- **Codeforces-style rank** based on overall completion, with a progress bar and "topics to next rank" hint
- **Flag for revision** (☆) to mark topics you want to revisit
- **Search and filters** by name, status (remaining, completed, flagged) and priority
- **Per-section progress** with a sidebar for quick navigation
- **Auto-saves** progress in your browser (`localStorage`)
- **Export / import** progress as JSON for backups or moving between machines
- **Light and dark mode** that follows your system setting
- **Zero dependencies**: one HTML file, no build step, no server
---
 
## Getting started
 
### Run locally
 
```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```
 
Then open `dsa-tracker.html` in any modern browser (Chrome, Firefox, Edge, Safari).
 
### Host on GitHub Pages (optional)
 
1. Rename `dsa-tracker.html` to `index.html`.
2. Go to **Settings → Pages** in your repository.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. Your tracker will be live at `https://<your-username>.github.io/<repo-name>/`.
---
 
## How to use
 
1. Tick a topic only when you can **explain it**, **recognize when to use it**, **implement it without help** and **state its time and space complexity**.
2. Flag topics with ☆ that need another pass.
3. Use **Remaining** + **P0 only** filters to see what to study next.
4. Click **Export progress** regularly to save a backup `.json` file.
> **Note:** Progress is stored in the browser you open the file in. Clearing browser data or switching browsers starts fresh, so keep an exported backup.
 
---
 
## Coverage
 
| Section | Priority |
|---|---|
| A. Arrays, searching and sorting | P0 |
| B. String algorithms | P1 |
| C. Linked lists, stacks and queues | P0 |
| D. Binary search and search patterns | P0 |
| E. Trees and binary search trees | P0 |
| F. Heaps and priority queues | P0 |
| G. Graph algorithms | P0 |
| H. Tries and prefix structures | P1 |
| I. Range queries and specialized data structures | P1 |
| J. Recursion and backtracking | P0 |
| K. Greedy algorithms and intervals | P0 |
| L. Dynamic programming | P0 |
| M. Bit manipulation | P1 |
| N. Math and number theory | P1 |
| O. Computational geometry | P2 |
| P. Advanced algorithm design and theory | P2 |
| Q. Core data structures inventory | Mixed |
| R. Complexity analysis and interview fundamentals | P0 |
| Interview readiness | P0 |
| Gaps: interview-critical patterns | P0 |
| Gaps: Codeforces 1500 to 2000+ | P1 |
| Gaps: advanced (2000+) | P2 |
 
### Rank tiers
 
| Completion | Rank |
|---|---|
| 0–14% | Newbie |
| 15–29% | Pupil |
| 30–49% | Specialist |
| 50–69% | Expert |
| 70–84% | Candidate Master |
| 85–99% | Master |
| 100% | Grandmaster |
 
---
 
## Suggested study order
 
| Phase | Focus | Time |
|---|---|---|
| 1 | Arrays, strings, hashing, two pointers, sliding windows, binary search, linked lists, stacks and queues | 2–3 weeks |
| 2 | Trees, heaps, graph traversal, shortest paths, Union-Find | 2–3 weeks |
| 3 | DP, greedy, backtracking, intervals, string algorithms, range-query structures | 3–4 weeks |
| 4 | Timed practice, mixed problems, revision and mock interviews | 2 weeks + ongoing |
 
---
 
## Customizing
 
All topics live in the `SECTIONS` array inside the `<script>` tag of the HTML file. To add a topic, append a string to a section's `items` list. To add a section, add a new object:
 
```js
{ id: "my-section", title: "My new section", pri: "P1", items: ["Topic one", "Topic two"] }
```
 
Keep each section `id` unique. Renaming an existing topic resets its saved tick, since progress is keyed by topic name.
 
---
 
## Resources
 
- [LeetCode problem set](https://leetcode.com/problemset/)
- [NeetCode roadmap](https://neetcode.io/roadmap)
- [Codeforces](https://codeforces.com/)
- [CP-Algorithms](https://cp-algorithms.com/)
- [Google Interview University](https://github.com/jwasham/coding-interview-university)
- [GeeksforGeeks](https://www.geeksforgeeks.org/)

 
