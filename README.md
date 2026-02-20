# RL Notes — Sutton & Barto

Personal study notes from *Reinforcement Learning: An Introduction* (Sutton & Barto, 2nd Ed.), built as a Quarto book and deployed to GitHub Pages.

## Live Site

[chizkidd.github.io/RL-Sutton-Barto-notes](https://chizkidd.github.io/RL-Sutton-Barto-notes)

## Chapters

| Chapter | Topic |
|---|---|
| 2 | Multi-Armed Bandits |
| 3 | Finite Markov Decision Processes |
| 4 | Dynamic Programming |
| 5 | Monte Carlo Methods |
| 6 | Temporal-Difference Learning |
| 7 | n-step Bootstrapping |
| 8 | Planning & Learning with Tabular Methods |

## Local Development

**Prerequisites:** [Quarto](https://quarto.org/docs/get-started/) installed.

```bash
# Clone the repo
git clone https://github.com/chizkidd/RL-Sutton-Barto-notes
cd RL-Sutton-Barto-notes

# Preview locally with live reload
quarto preview

# Build the static site
quarto render
```

Output goes to `_site/`.

## Deployment

Pushing to `main` automatically deploys to GitHub Pages via the GitHub Actions workflow in `.github/workflows/deploy.yml`.

To set up GitHub Pages for the first time:
1. Push the repo to GitHub
2. Go to **Settings → Pages → Source** and select **GitHub Actions**
3. Push a commit to `main` to trigger the first deploy

## Project Structure

```
RL-Sutton-Barto-notes/
├── _quarto.yml          # Book config, chapters list, theme
├── index.qmd            # Preface / landing page
├── custom.scss          # Custom styles (light + dark mode)
├── references.bib       # BibTeX references
├── chapters/            # One .qmd file per chapter
│   ├── ch02-multi-armed-bandits.qmd
│   ├── ch03-finite-mdps.qmd
│   └── ...
└── figures/             # figure diagrams
    ├── ch06-6-4-sarsa.png
    └── ...
```

## Reference

Sutton, R. S., & Barto, A. G. (2018). *Reinforcement Learning: An Introduction* (2nd ed.). MIT Press.
