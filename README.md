# Technical English Writing Toolkit

Interactive writing practice for engineering students (B2–C1) at Universitat
Politècnica de València. Twenty-seven self-marking tools and 558 exercises, in four sections.

Designed by Ruzana Galstyan-Sargsyan.

## What this is

Every tool opens on practice, marks itself instantly, and explains every answer.
A reference tab holds the rules; several tools end with a scaffold or draft the
student copies into their own work.

Nothing is saved and nothing is sent anywhere — no accounts, no cookies, no
analytics. Scores reset on reload. Every page prints cleanly.

## The files

```
index.html                                the hub
README.md

academic-writing/
  cars-model-introductions.html           Writing an Introduction
  technical-report-structure.html         What Goes in Each Section
  describing-data-and-trends.html         Writing About Your Results
  paraphrasing-and-citing.html            Using Sources Without Copying
  reporting-verbs.html                    Choosing Your Citation Verb
  evaluating-sources.html                 Is This Source Worth Citing?
  verb-tenses-by-section.html             Verb Tenses by Section
  active-or-passive.html                  Active or Passive?
  modals-in-technical-writing.html        Modals: Must, Should, May
  analysing-hedging-language.html         How Certain Should You Sound?

technical-writing/
  describing-a-mechanism.html             Describing a Mechanism
  describing-a-process.html               Explaining How Something Works
  lab-reports.html                        Lab Reports
  progress-reports.html                   Progress Reports
  proposals.html                          Proposals
  recommendation-reports.html             Recommendation & Feasibility
  apa-7-referencing.html                  APA 7 Referencing
  problem-solving-emails.html             Problem-Solving Emails
  professional-emails.html                Emails That Get a Reply

presentations/
  presenting-technical-work.html          Giving a Technical Presentation
  slides-that-work.html                   Slides That Work
  presenting-as-a-team.html               Presenting as a Team

ai-ethics/
  ai-writing-scenarios.html               When Is AI Use Acceptable?
  ai-traffic-lights.html                  Sorting AI Use into Three Bands
  thinking-with-ai.html                   Using AI as a Critic
  prompt-builder.html                     Asking Better Questions
  human-or-ai-writing.html                Spotting Empty Prose
```

Twenty-nine files in four folders. All self-contained: each is one HTML file with its
own CSS and JavaScript inside. No framework, no build step, no server, no external
requests.

## Publishing

1. Create the four folders in your repository and upload each set of files into its
   own folder. `index.html` and `README.md` go at the **root**, not in a folder.
2. **Settings → Pages** → Source: *Deploy from a branch* → Branch: `main`,
   folder: `/ (root)` → **Save**.
3. Wait two or three minutes. The live link appears at the top of that page.

**Uploading folders on github.com:** click **Add file → Upload files**, then drag the
whole `academic-writing` folder in — GitHub keeps the folder structure. Repeat for
each folder, or drag all four at once.

To update a tool later, upload it into the same folder with the same name; it replaces
the old version. Then hard-refresh (Ctrl+Shift+R) — browsers cache aggressively.

**A warning about moving files.** Links inside the tools use relative paths —
`../index.html` for the hub, `../technical-writing/lab-reports.html` across folders.
If you move a file to a different folder, its links break. Tell me instead and I will
rewrite them.

## Section colours

| Section | Variable | Colour |
|---|---|---|
| Academic writing | `--f-acad` | `#2F5FA8` blue |
| Technical writing | `--f-tech` | `#B07A1E` ochre |
| Presentations | `--f-pres` | `#6B4E9E` violet |
| AI ethics in writing | `--f-ai` | `#2E6E6B` teal |

Each tool repeats its section colour near the top of its own file as `--accent`,
with a pale tint as `--accent-soft`. Change a section colour in both places.

## Adding a tool

Copy the closest existing tool, rename it (lowercase, hyphens, **no spaces** —
spaces become `%20` and break links pasted into PoliformaT or Teams), then replace
the `Q` array in the script with your own exercises and rewrite the reference tab.
Add a card in `index.html` copying an existing one. The `data-keywords` attribute
feeds the search box.

## Credits and licences

- **Technical writing** tools are adapted in part from Last, S. (2019).
  [*Technical Writing Essentials*](https://pressbooks.bccampus.ca/technicalwriting/).
  University of Victoria. Licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
  Individual tools name which chapter and what was changed.
- **AI ethics in writing** tools are based on Cheng, A., Calhoun, A., & Reedy, G.
  (2025). Artificial intelligence-assisted academic writing: recommendations for
  ethical use. *Advances in Simulation*, 10(1), 22.
  <https://doi.org/10.1186/s41077-025-00350-6> — open access.
- Other tools draw on Swales & Feak, Hyland, and the University of Manchester
  Academic Phrasebank; each names its sources on its own Source tab.
- The hub format was inspired by
  [Hamid Guedra's HTML Tools](https://hamgued.github.io/html-tools/) at LAB
  University of Applied Sciences.

## A note on the examples

Studies, authors, companies, faults and figures throughout were written for
teaching. They are realistic but invented, and should not be cited.
