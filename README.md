# Equine-Corneal-Anesthesia-Analysis

R workflow for a two-period crossover study comparing dexmedetomidine + ropivacaine, ropivacaine, and saline in standing horses.   Includes data-wrangling scripts, mixed-effects &amp; Wilcoxon analyses, full report (R Markdown → PDF), Beamer talk, CURC poster, and reproducible figures/tables.
---

##   Contents
| folder / file | purpose |
|---------------|---------|
| `data/` | **Excel workbook** with “Full”, “Summarized”, and “HemScore” sheets (not tracked – add to `.gitignore` & provide a link) |
| `R/` | all R scripts & helper functions |
| `report/Report_Draft.Rmd` → `pdf` | 20-page manuscript with numbered sections & appendix code |
| `presentation/horse_eyes_presentation.Rmd` → `pdf` | 10-min Beamer slide deck |
| `poster/` | CURC tri-fold poster (PowerPoint & exported PDF) |
| `figs/` | publication-ready PNG/PDF figures (EMMeans plot, spaghetti plot, time-course ribbons, hemorrhage bar) |
| `LICENSE` | MIT |

---

##  Quick start

```bash
# clone repo
git clone https://github.com/your-user/equine-corneal-anesthesia-analysis.git
cd equine-corneal-anesthesia-analysis

# open R
renv::restore()          # reproducible package versions
rmarkdown::render("report/Report_Draft.Rmd")
rmarkdown::render("presentation/horse_eyes_presentation.Rmd")
