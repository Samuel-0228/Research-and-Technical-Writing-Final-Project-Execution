# Social Media as an Unofficial Advisory System: Trust and Reliance on Crowdsourced Academic Advice Among AAU Undergraduate Students

**Course:** Research and Technical Writing for Information Systems (INSY 3061) - Section 2, Group 11 
**Institution:** Addis Ababa University, College of Natural and Computational Sciences, Department of Information Systems 
**Advisor:** Dr. Ermias Abebe 
**Submission Due Date:** December 13, 2026 
**Repository Deadline:** November 25, 2026 
**GitHub Repository URL:** [https://github.com/Samuel-0228/Research-and-Technical-Writing-Final-Project-Execution](https://github.com/Samuel-0228/Research-and-Technical-Writing-Final-Project-Execution) 

---

## Group Members

| Full Name | Student ID |
| :--- | :--- |
| Feyisa Gezahegn | UGR/4624/17 |
| Samuel Debasu | UGR/0995/17 |
| Samuel Yeshambel | UGR/5294/17 |
| Temesgen Yohannes | UGR/4291/17 |
| Yabtsega Belete | UGR/9879/17 |

---

## Project Overview

Undergraduate students at Addis Ababa University (AAU) frequently make high-stakes academic decisions - such as course registration, instructor evaluation, and freshman department placement - under significant information scarcity. When formal institutional advising channels fall short or prove cumbersome, students increasingly turn to batch- and department-specific Telegram channels. Within these environments, students form an **unofficial, crowdsourced advisory system** operating without institutional oversight or quality control.

This research investigates:
1. **Source Trust vs. Reliance (RQ1):** How AAU undergraduates evaluate the trustworthiness (ability, benevolence, integrity) of three distinct peer source types - **seniors**, **friends/classmates**, and **anonymous posters** - and how this trust predicts actual reliance on peer advice.
2. **Academic Decisions & Misguidance (RQ2):** Which specific academic decisions are most heavily swayed by crowdsourced peer guidance, and what concrete challenges or adverse outcomes students encounter when acting on inaccurate or outdated advice.

---

## Repository Structure

In strict compliance with the course project guidelines, this repository is organized into the following standardized folder structure:

```
research-final/
│
├── proposal/ # Approved proposal documentation (PDF, DOCX, and summary)
├── instruments/ # Data collection instruments, survey scales, and administration guide
├── pilot-study/ # Pilot testing protocol, cognitive interview feedback, and revisions
├── data/ # Raw and processed datasets, codebook, and anonymization logs
│ ├── raw/ # Raw, untransformed survey responses (anonymized)
│ └── processed/ # Cleaned, coded datasets ready for statistical analysis
├── analysis/ # Analysis pipeline scripts, requirements, and generated outputs
│ └── outputs/ # Regression tables, reliability reports, charts, and figures
├── report/ # Final research report draft, contribution statement, AI declaration
├── presentation/ # Final defense slide deck outline and presentation materials
├── meeting-notes/ # Weekly meeting agendas, team discussion records, and action items
├── references/ # APA 7th edition bibliographic database (BibTeX) and literature matrix
├── .gitignore # Version control exclusions for clean project history
└── README.md # Project overview, directory guide, and reproduction instructions
```

### Folder Directory Breakdown

| Directory | Purpose & Required Artifacts |
| :--- | :--- |
| [`proposal/`](file:///home/lap/Downloads/thefolders/research-final/proposal/) | Houses the instructor-approved research proposal (`approved_proposal.pdf`), editable revisions (`proposal_revised.docx`), and a markdown summary of objectives and scope. |
| [`instruments/`](file:///home/lap/Downloads/thefolders/research-final/instruments/) | Contains the operationalized measurement instruments (`questionnaire.md`), adapted constructs (Mayer et al. trust dimensions, Information Adoption Model), and survey distribution protocols. |
| [`pilot-study/`](file:///home/lap/Downloads/thefolders/research-final/pilot-study/) | Documents the initial pilot study ($N = 10$), debriefing logs, clarity/ambiguity feedback, and the audit trail of modifications made to the instruments. |
| [`data/`](file:///home/lap/Downloads/thefolders/research-final/data/) | Houses data management documentation, the complete variable codebook (`codebook.md`), and segregated raw/processed data storage adhering to research ethics. |
| [`analysis/`](file:///home/lap/Downloads/thefolders/research-final/analysis/) | Contains executable Python analysis scripts (`analysis_pipeline.py`), dependency definitions (`requirements.txt`), and reproduction steps for regression and ANOVA models. |
| [`report/`](file:///home/lap/Downloads/thefolders/research-final/report/) | Contains the final academic research report manuscript, Group Contribution Statement (1-page max), AI Usage Declaration, and Ethics Statement. |
| [`presentation/`](file:///home/lap/Downloads/thefolders/research-final/presentation/) | Stores the group's final presentation slide deck, speaker allocations, and presentation structure. |
| [`meeting-notes/`](file:///home/lap/Downloads/thefolders/research-final/meeting-notes/) | Demonstrates continuous collaborative workflow through dated logs of group deliberations, decisions, and weekly sprint commitments. |
| [`references/`](file:///home/lap/Downloads/thefolders/research-final/references/) | Comprehensive bibliographic database in BibTeX format (`references.bib`), APA 7th edition reference list, and a synthesized literature matrix. |

---

## Software, Tools & Datasets Used

- **Survey Administration:** Google Forms / Telegram Bot WebApp (with soft quota sampling across AAU departments and academic batches).
- **Statistical Analysis:** Python 3.10+ (`pandas`, `numpy`, `scipy`, `statsmodels`, `pingouin`, `matplotlib`, `seaborn`) / SPSS.
- **Reference Management:** BibTeX, Zotero (formatted according to APA 7th Edition standards).
- **Version Control:** Git & GitHub (collaborative branching, code/data reviews, and iterative commits).
- **Dataset:** Primary survey dataset of $N \approx 150\text{--}200$ AAU undergraduate students.

---

## Reproduction & Analysis Instructions *(Phase 4 Workflow)*

Once primary survey collection is completed in Phase 3, the statistical analysis and artifact generation will be executed using the following steps:

### 1. Clone the Repository
```bash
git clone https://github.com/Samuel-0228/Research-and-Technical-Writing-Final-Project-Execution.git
cd Research-and-Technical-Writing-Final-Project-Execution
```

### 2. Set Up a Virtual Environment & Install Dependencies
```bash
python3 -m venv venv
source venv/bin/activate # On Windows use: venv\Scripts\activate
pip install -r analysis/requirements.txt
```

### 3. Run the Statistical Pipeline
```bash
python analysis/analysis_pipeline.py
```
This script will:
- Validate dataset integrity and inspect missing values.
- Calculate internal consistency reliability (Cronbach's $\alpha$) across all multi-item constructs.
- Perform descriptive statistical summaries across demographic strata.
- Conduct repeated-measures ANOVA / pairwise tests comparing perceived trust across seniors, friends, and anonymous contributors.
- Estimate Ordinary Least Squares (OLS) multiple linear regression models predicting student reliance on crowdsourced advice.
- Generate high-resolution figures and tabular summaries directly into `analysis/outputs/`.

---

## Project Timeline & Milestones

- **November 22, 2026:** Assignment launch & Git repository initialization.
- **November 25, 2026:** Official repository URL submission on Google Classroom.
- **November 26 - 28, 2026:** Instrument refinement and pilot study administration ($N=10$).
- **November 29 - December 06, 2026:** Large-scale primary data collection across AAU Telegram channels.
- **December 07 - 09, 2026:** Data cleaning, coding, reliability analysis, and regression modeling.
- **December 10 - 12, 2026:** Research report drafting, peer review, and presentation slide deck preparation.
- **December 13, 2026:** **Final Submission Deadline** (Report PDF, Repository, Slides, and Declarations).
