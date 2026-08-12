# Push Instructions — StrayDogSyn Profile Repo

## Before you push: one blocking item

Open `README.md`, search for `REPLACE-WITH-ARTICLE-URL`, and paste the real MassLive
article URL from The Last Mile newsletter. MassLive blocks automated fetching, so I
could not retrieve it. There is an HTML comment above the badge marking the spot.

If you would rather drop the press badge entirely, delete the two lines between the
`WRITING & PRESS` comment and the table that follows it, plus the right-hand cell of
that table.

---

## What is in this folder

```
README.md                                   → replaces the repo root README.md
docs/AISE-Manifesto.pdf                     → new file
docs/Justice-Through-Code-Certificate.pdf   → new file
```

The README links to both PDFs at these exact paths, so keep the `docs/` folder name.

---

## Commands

From the root of your local `StrayDogSyn/StrayDogSyn` clone:

```bash
# 1. make sure you are current
git checkout main
git pull origin main

# 2. copy the files in (adjust the source path to wherever you saved this folder)
mkdir -p docs
cp /path/to/StrayDogSyn-profile/README.md            ./README.md
cp /path/to/StrayDogSyn-profile/docs/*.pdf           ./docs/

# 3. confirm what changed before committing
git status
git diff --stat

# 4. commit and push
git add README.md docs/AISE-Manifesto.pdf docs/Justice-Through-Code-Certificate.pdf
git commit -m "Add AISE Manifesto and JTC certificate; restructure projects and accomplishments

- Publish The AISE Manifesto and Justice Through Code certificate under docs/
- Rename Currently Working On to Recent Accomplishments
- Swap CompTIA card for Lead By Example, bookend with Second Story
- Add StrayDog Syndications LLC and Python Essentials to Featured Projects
- Move MERN Pomodoro and MovieBuzz to More Projects
- Replace LangChain badge with ChatGPT and Codex
- Document LangChain, MCP servers, and AI orchestration familiarity
- Add in-document navigation anchors"

git push origin main
```

PowerShell equivalent for steps 2 and 3:

```powershell
New-Item -ItemType Directory -Force -Path docs
Copy-Item "C:\path\to\StrayDogSyn-profile\README.md" -Destination ".\README.md" -Force
Copy-Item "C:\path\to\StrayDogSyn-profile\docs\*.pdf" -Destination ".\docs\" -Force
git status
```

---

## After pushing — verify these five things

1. The nav links under the social badges jump to the right sections.
2. `docs/AISE-Manifesto.pdf` renders in GitHub's inline PDF viewer.
3. The Justice Through Code card opens the certificate.
4. The two private-repo badges show as grey `Private Repo` (they will 404 for
   logged-out visitors, which is expected and correct).
5. The ChatGPT and Codex badges render — both use the `openai` shields.io logo
   slug, since shields has no dedicated Codex icon.

---

## Known discrepancy to resolve on your side

The live Python Essentials site links its source to
`StrayDogSyn/Python-Essentials-Code-The-Dream`, but you gave me
`StrayDogSyn/Python-Essentials-Bridge-The-Dream` as the private repo. I used the one
you gave me. If those are two different repositories, decide which one the README
should point at.
