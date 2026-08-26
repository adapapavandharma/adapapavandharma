## Pavan Dharma Adapa

Healthcare and research data analyst. M.S. Computer Science, Mississippi State University.
Currently a Data Analytics Intern in the Agricultural Microbiomes Lab at MSU.

I work on the unglamorous layer analysis actually rests on — validated pipelines,
reproducible results, and checks that fail loudly instead of quietly. Every project
below states what it found, how it was verified, and where it fell short.

Work-authorized through June 2027 on F-1 OPT, STEM-extension eligible to 2029.
Open to relocation. **Available now.**

---

### Open-source contribution

**[nano16s](https://github.com/lz245/nano16s)** — Oxford Nanopore full-length 16S rRNA
taxonomic profiling. The tool belongs to the Agricultural Microbiomes Lab; I authored
**[all 30 merged pull requests](https://github.com/lz245/nano16s/pulls?q=is%3Apr+author%3Aadapapavandharma+is%3Amerged)**
that took it from a cluster-bound research script to a documented tool that installs and
runs on an ordinary laptop:

- continuous integration, packaging, and a per-run performance report
- cross-platform support — Linux, macOS, WSL2, managed Windows
- failure diagnostics that name the real cause (host clock drift, an empty barcode, a
  length window that does not fit the amplicon) instead of the misleading error
- data-correctness fixes: the right abundance table, stray files no longer become
  samples, a failed database rebuild no longer destroys a working one
- a user guide written from an unprepared machine forward, plus contributor docs and linting

---

### Health data projects

**[clinical-quality-measures](https://github.com/adapapavandharma/clinical-quality-measures)**
— HEDIS / CMS eCQM engine over a 13,810-patient synthetic EHR (820,993 encounters,
10.8M observations). Measures are **data, not code**: each is a YAML spec with its
SNOMED CT and LOINC value sets held separately, so an annual steward update is a
reviewable diff rather than a code change with regression risk.

**[denials-analytics](https://github.com/adapapavandharma/denials-analytics)**
— Three years of CMS Transparency in Coverage filings: 15,545 plan-years, **126.9M denied
claims**. Only 0.168% are ever appealed, and 40.1% of appeals are overturned. The
bottleneck is capacity to file, not claim merit.

**[ed-throughput-analytics](https://github.com/adapapavandharma/ed-throughput-analytics)**
— 16,025 real CDC/NCHS emergency department visits, survey-weighted to **155,397,747**
national visits. The pipeline refuses to run unless it reproduces CDC's published total.
Between-hospital variation in door-to-provider time is **3.9× larger** than between-hour
variation — it isn't *when*, it's *where*. The peak-hour effect I expected did not
survive the weighting, and I reported that as a null result.

**[readmission-risk](https://github.com/adapapavandharma/readmission-risk)**
— 30-day readmission over 99,343 real inpatient encounters. AUC is 0.664, and the point
of the project is that AUC is the wrong thing to judge it on: working the **top 20% of
the risk list catches 37.7% of all readmissions**, at 1.89× enrichment and a
number-needed-to-screen of 4.8.

**[experimentation-toolkit](https://github.com/adapapavandharma/experimentation-toolkit)**
— Five ways A/B tests quietly fail, each measured against known ground truth rather than
asserted. Peeking ten times at a null experiment drives the false positive rate to
**18.5%** against a nominal 5%. CUPED at ρ=0.7 is worth 1.96× the traffic at no cost.

---

### Toolkit

`Python` `SQL` `R` · pandas, NumPy, SciPy, scikit-learn · PostgreSQL, MySQL, SQLite
Power BI, Tableau · Git, CI · SNOMED CT, LOINC, ICD-10, HEDIS/eCQM · Linux, WSL2

---

**[Portfolio](https://adapapavandharma.github.io)** ·
**[LinkedIn](https://linkedin.com/in/adapapavandharma)** ·
adapapavandharma@gmail.com
