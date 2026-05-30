# How-To-Train-Your-Researcher

A compilation of advice on how to do AI research (e.g., reading academic papers, writing proposals, or scoping for experiments) from researchers in Singapore. The mainpage (HTTYR) is also the official documentation for the Early Research Opportunity Program organized by [Singapore Youth AI](https://sgyouthai.org/).

**Live site:** https://how-to-train-your-researcher.github.io/HTTYR

---

## Repository structure

```
├── _quarto.yml               # site configuration (theme, navbar, bibliography)
├── index.qmd                 # HTTYR landing page
├── advice/
│   ├── erop.qmd              # EROP Playbook — program curriculum and mentoring strategy
│   ├── reading_advice.qmd    # Reading Advice — how to read research papers
│   └── writing_advice.qmd    # Writing Advice — academic writing techniques
├── attachments/              # images and screenshots referenced in advice/*
├── references.bib            # shared BibTeX bibliography
└── styles.css                # custom CSS overrides
```

#### What is a `.qmd` file?

A `.qmd` (Quarto Markdown) file is a plain-text file, very similar to a standard `.md` (Markdown) file, with a few extras:

- **YAML front matter** (between `---` fences at the top) sets the title, authors, and date.
- **Markdown body** — headings, bold, italics, tables, bullet lists, links — exactly as in GitHub-flavoured Markdown.
- **LaTeX math** inline with `$...$` or display with `$$...$$`.
- **Citations** with `[@bibtex-key]` — keys come from `references.bib`.
- **Callout blocks** for tips, notes, and warnings (e.g., `::: {.callout-tip}`).

You do **not** need to install Quarto to contribute text. Edit the `.qmd` files as you would any Markdown file.

---

## How to contribute!

Contributions are welcomed! The two advice most open to community inputs are:

| File | What to add |
|---|---|
| `advice/reading_advice.qmd` | Tips on reading AI research papers — personal strategies, useful questions to ask, tools you used.  |
| `advice/writing_advice.qmd` | Academic writing techniques — sentence patterns, signposting moves, hedging strategies etc. |

The `index.qmd` and `advice/erop.qmd` files are maintained primarily by the EROP team.

### Step-by-step

1. **Fork** this repository on GitHub.
2. **Edit** the relevant `.qmd` file in the `advice/` folder. Find the section marked with `> *(Contributions welcome...)*` and replace or extend it.
3. **Add images** (if any) to the `attachments/` folder and reference them in the guide with:
   ```markdown
   ![Caption](../attachments/your-image.png){fig-align="center" width="80%"}
   ```
4. **Add references** (if any) to `references.bib` in BibTeX format, then cite with `[@your-key]` in the text.
5. **Open a pull request** against `main` with a short description of what you added and why.

### Style guidelines

- Write in plain, direct English.
- One idea per paragraph. Start each paragraph with a topic sentence that states the claim.
- Use callout blocks (`::: {.callout-tip}`) to highlight actionable advice.
- Do not restructure existing sections without prior discussion — open an issue first.
