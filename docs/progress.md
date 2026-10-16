# PathToC – Mentor Progress Tracker

Paste this whole file into a new chat with Claude if you ever start a fresh conversation.

## About me
- MSc Data Science student, Northumbria University (Newcastle, UK)
- 1 hour per day for extra study, 6 days a week (Sunday off)
- Goal: employable in Data Science / AI / ML, plus one serious startup-style portfolio project
- Laptop: Windows, VS Code, Python 3.13.7, Git installed
- Mentor format: daily sessions = 10–15 min learn, 30–40 min build, 5–10 min review, one test question, what to do tomorrow

## The project: PathToC
- Helps UK private landlords find which rental homes fail the EPC band C standard (deadline 1 Oct 2030) and the cheapest path to C.
- Key detail: homes rated C on the current EPC rating before 1 Oct 2029 count as compliant until that EPC expires.
- Data: government EPC open data (https://get-energy-performance-data.communities.gov.uk/, GOV.UK One Login), starting with Newcastle upon Tyne.
- Planned stack: Python, pandas, DuckDB (week 1), PostgreSQL, scikit-learn + LightGBM + SHAP, FastAPI, Streamlit, Docker, GitHub Actions; LLM explainer later.

## Links
- GitHub profile: https://github.com/abzal-shaik-ds
- Project repo: https://github.com/abzal-shaik-ds/pathtoc
- Local folder: D:\Projects\pathtoc
- Start each session: open VS Code in D:\Projects\pathtoc, run .venv\Scripts\activate

## Progress log
### Day 1 – Fri 16 Oct 2026 – DONE
- Renamed GitHub username to abzal-shaik-ds; filled profile bio
- Installed Git; set git user.name / user.email
- Created pathtoc repo (README, Python .gitignore, MIT licence)
- Created .venv; installed pandas, duckdb, jupyter; requirements.txt
- Folders: data/raw, docs, notebooks, src; added data/ to .gitignore
- Wrote docs/problem.md and docs/log.md; first commit pushed
- Open: answer test question – "Why should raw data stay out of Git, and how could someone else reproduce your work without it?"
- Moved to Day 2: download EPC data

### Day 2 – NEXT
1. Sign in with GOV.UK One Login and download domestic EPC data (Newcastle if possible, else full file) into data/raw/
2. Learn pandas .info(), .isna().sum(), .value_counts()
3. notebooks/01_first_look.ipynb: shape, dtypes, missing values, current rating distribution, 5 written observations
4. Test question: why might the same house appear several times?

### Upcoming (week 1)
- Day 3: data dictionary (15 key columns) + licence summary -> docs/data_dictionary.md
- Day 4: 5 competitor tools -> docs/market.md
- Day 5 (Fri): DuckDB SQL (counts, ROW_NUMBER latest cert per property) + shortlist 5 grad schemes/internships
- Day 6: % of rented Newcastle homes below C by construction age band + one chart; weekly review
- Day 7: rest (optional: list 10 Newcastle letting agents)

## Still to tell my mentor
- When my MSc ends
- My Python and SQL level out of 5