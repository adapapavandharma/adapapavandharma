## Pavan Dharma Adapa

Research and health data analyst. M.S. Computer Science, Mississippi State University, May 2026.
Currently a Data Analytics Intern in the Agricultural Microbiomes Lab at MSU.

I clean, validate and document research and health data so the results can be checked.
Each project below names its data source and states what it found, how it was verified,
and where it fell short.

Authorized to work in the U.S. Open to relocation.
**Available now.**

---

### Health data projects

Self-directed and public. Each one names its data source.

**[ed-throughput-analytics](https://github.com/adapapavandharma/ed-throughput-analytics)**:
16,025 real CDC/NCHS emergency department visits, survey-weighted to **155,397,747**
national visits. The pipeline refuses to run unless it reproduces CDC's published total.
Between-hospital variation in door-to-provider time is **3.56× larger** than between-hour
variation. It isn't *when*, it's *where*. The peak-hour effect I expected did not survive
the weighting, and I reported that as a null result.

**[clinical-quality-measures](https://github.com/adapapavandharma/clinical-quality-measures)**:
HEDIS / CMS eCQM engine over a 13,810-patient Synthea synthetic, non-PHI EHR (820,993
encounters, 10.8M observations). Measures are **data, not code**. Each is a YAML spec with
its SNOMED CT and LOINC value sets held separately, so an annual steward update is a
reviewable diff rather than a code change. In the diabetes poor-control measure, 203 of the
204 patients in the numerator had no HbA1c test on record. That is an artifact of how the
Synthea generator schedules labs, so I report it as a check on the engine, not a finding
about care.

**[readmission-risk](https://github.com/adapapavandharma/readmission-risk)**:
30-day readmission over 99,343 real de-identified inpatient encounters. AUC is 0.664, and
the point of the project is that AUC is the wrong thing to judge it on. Working the
**top 20% of the risk list catches 37.7% of all readmissions**, at 1.89× enrichment and a
number-needed-to-screen of 4.8.

**[denials-analytics](https://github.com/adapapavandharma/denials-analytics)**:
Three years of real CMS Transparency in Coverage filings: 15,545 plan-years, **126.9M
denied claims**. Only 0.168% of denials are ever appealed, and 40.1% of appeals are
overturned. The pattern holds across all three years.

---

### Research

**Graduate Research Assistant**, Mississippi State University, Aug 2024 to Aug 2025.
Cleaned and analyzed a 900,000+ record Vesicular Stomatitis Virus (VSV) livestock-outbreak
dataset for Computer Science and Veterinary Medicine faculty. Built a Python/Selenium
scraper that collected genome metadata for a poultry respiratory-disease project, cutting
collection from hours to under 10 minutes per dataset.

**Publication.** Co-author (third of five) on *Computational Tools for Modeling and
Predicting Respiratory Disease Spread in Commercial Poultry Production*, a review article
under revision after peer review. I contributed the data preparation, statistical modeling
and results reporting, and drafted technical sections.

---

### Open-source contribution

**[nano16s](https://github.com/lz245/nano16s)**: Oxford Nanopore full-length 16S rRNA
taxonomic profiling. The tool belongs to the Agricultural Microbiomes Lab, and Li Zhang
maintains it. I authored
**[all 36 merged pull requests](https://github.com/lz245/nano16s/pulls?q=is%3Apr+author%3Aadapapavandharma+is%3Amerged)**
and 57 of its 68 non-merge commits. Together they took it from a cluster-bound research
script to a documented tool that installs and runs on an ordinary laptop:

- continuous integration, packaging, and a per-run performance report
- cross-platform support: Linux, macOS, WSL2, managed Windows
- failure diagnostics that name the real cause (WSL2 clock drift, an empty barcode, a
  length window that does not fit the amplicon) instead of the misleading error
- data-correctness fixes: the right abundance table, stray files no longer become
  samples, a failed database rebuild no longer destroys a working one
- a user guide written from an unprepared machine forward, plus contributor docs and linting

---

### Also

**[experimentation-toolkit](https://github.com/adapapavandharma/experimentation-toolkit)**:
outside healthcare. Five ways A/B tests quietly fail, each measured by simulation against
known ground truth. Peeking ten times at a null experiment drives the false positive rate
to **18.5%** against a nominal 5%. CUPED at rho 0.7 cuts variance 49%, which is worth 1.96×
the traffic.

---

### Toolkit

`Python` `SQL` `R` `Bash` · pandas, NumPy, SciPy, scikit-learn · survey-weighted estimation ·
SQLite, star schemas, dimensional modeling · Snakemake · pytest, GitHub Actions CI ·
Power BI, Google Analytics 4 · HEDIS/eCQM, SNOMED CT, LOINC · Linux, macOS, WSL2

---

**[Portfolio](https://adapapavandharma.github.io)** ·
**[LinkedIn](https://linkedin.com/in/adapapavandharma)** ·
adapapavandharma@gmail.com
