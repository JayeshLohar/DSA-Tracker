# DSA Prep Trackers

Two offline checklists for coding-interview and competitive programming preparation. Each is a single HTML file: no install, no server, no dependencies. Open it in a browser, tick items as you master them, and track your progress over time.

| File | What it tracks | Items |
|---|---|---|
| `dsa-tracker.html` | Algorithms, data structures and problem-solving patterns, tagged P0 / P1 / P2 | 383 |
| `design-tracker.html` | Data-structure and low-level design questions, tagged Easy / Medium / Hard | 168 |

---

## Features

- **Checkboxes with progress bars** for every section, plus an overall progress bar
- **Codeforces-style rank** (Newbie → Pupil → Specialist → Expert → Candidate Master → Master → Grandmaster) based on how much you've completed
- **Flag for revision** with ☆ on any item you want to revisit
- **Search and filters** by name, status (remaining, completed, flagged) and priority or difficulty
- **Sidebar navigation** to jump between sections, with collapsible sections
- **Auto-save** in your browser, so your ticks are still there next time
- **Export / import** progress as a JSON file for backups or moving to another machine
- **Light and dark mode** that follows your system setting

---

## What's inside

### DSA tracker

Covers the core topics from a FAANG-level DSA checklist:

- Arrays, searching and sorting
- Strings (KMP, Z-algorithm, rolling hash, suffix arrays)
- Linked lists, stacks, queues and monotonic structures
- Binary search, trees, heaps and tries
- Graphs (BFS/DFS, shortest paths, Union-Find, MST, SCC, flows)
- Range queries (Fenwick tree, segment tree, sparse table)
- Recursion, backtracking, greedy and intervals
- Dynamic programming, from 1D/2D up to DP optimizations
- Bit manipulation, number theory and computational geometry
- Complexity analysis and interview fundamentals

It also includes three **gap sections** for topics often missing from standard lists: interview-critical patterns (two pointers, sliding window, prefix sum + hash map, design-style problems), Codeforces 1500 → 2000+ techniques, and advanced 2000+ topics.

**Priorities:** P0 = must master, P1 = important, P2 = advanced or specialized.

### Design tracker

Covers "design a class / data structure" questions common in interviews:

- **Easy:** stacks, queues, HashMap, circular queue, heaps, rate logger
- **Medium:** LRU Cache, Twitter, Time-Based KV Store, iterators, calendars, Snapshot Array; low-level design such as TTL cache, transactions, parking lot, order book and Splitwise; concurrency problems such as Print in Order and Producer-Consumer
- **Hard:** LFU Cache, All O(1), Autocomplete, Range Module, Skiplist, text editor, in-memory file system; advanced systems such as LSM tree, consistent hashing, thread pool and matching engine

---

## Getting started

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

Open `dsa-tracker.html` or `design-tracker.html` in Chrome, Firefox, Edge or Safari.

### Host on GitHub Pages (optional)

1. Go to **Settings → Pages** in the repository.
2. Choose **Deploy from a branch**, select `main` and `/ (root)`, and save.
3. Open `https://<your-username>.github.io/<repo-name>/dsa-tracker.html` (or `design-tracker.html`).

---

## How to use

1. **Tick an item only when you've truly learned it.**
   - For a DSA topic, you can explain it, recognize when to use it, implement it without help, and state its complexity.
   - For a design question, you can define the API, choose the data structures, justify each operation's complexity, and code it cleanly.
2. **Flag with ☆** anything that needs another pass.
3. **Filter by Remaining + P0 (or Easy)** to decide what to study next.
4. **Export progress regularly** to keep a backup.

> **Note:** Progress is saved in the browser where you open the file. Clearing browser data or switching browsers starts fresh, so keep an exported backup. The two trackers save progress separately.

---

## Suggested study order

| Phase | Focus | Time |
|---|---|---|
| 1 | Arrays, strings, hashing, two pointers, sliding window, binary search, linked lists, stacks, queues; Easy design questions | 2–3 weeks |
| 2 | Trees, heaps, graph traversal, shortest paths, Union-Find; Medium design questions | 2–3 weeks |
| 3 | DP, greedy, backtracking, intervals, string algorithms, range queries; Hard design questions | 3–4 weeks |
| 4 | Timed practice, mixed problems, revision and mock interviews | 2 weeks + ongoing |

---

## Customizing

All items live in the `SECTIONS` array inside each file's `<script>` tag. To add an item, append a string to a section's `items` list. To add a section:

```js
{ id: "my-section", title: "My new section", pri: "P1", items: ["Item one", "Item two"] }
```

Keep each section `id` unique. Renaming an item resets its saved tick, because progress is keyed by name.

---

## Resources

- [LeetCode](https://leetcode.com/problemset/)
- [NeetCode roadmap](https://neetcode.io/roadmap)
- [Codeforces](https://codeforces.com/)
- [CP-Algorithms](https://cp-algorithms.com/)
- [Google Interview University](https://github.com/jwasham/coding-interview-university)

---

## License

MIT
