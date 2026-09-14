# OPVA

**OPVA: A Facet-Activated Dataset for Personality and Competency Assessment in Asynchronous Video Interviews**

[Tianyi Zhang](https://tianyi-zhang-tz.github.io/Tianyi-Zhang-TZ/), Antonis Koutsoumpis, Janneke K. Oostrom, Djurre Holtrop, Sina Ghassemi, Reinout E. de Vries

Papers: [IEEE TAC 2024](https://doi.org/10.1109/TAFFC.2024.3374875) · [Computers in Human Behavior 2024](https://doi.org/10.1016/j.chb.2023.108128) 

## Links

| Resource | Link |
|----------|------|
| **Paper (IEEE TAC)** | https://doi.org/10.1109/TAFFC.2024.3374875 · [author PDF](https://tianyi-zhang-tz.github.io/Tianyi-Zhang-TZ/papers/LLMs_Personality.pdf) |
| **Paper (CHB)** | https://doi.org/10.1016/j.chb.2023.108128 |
| **Project Page** | [English](https://apal-seu.github.io/OPVA/), [中文](https://apal-seu.github.io/OPVA/zh.html) |
| **User Agreement** | [OPVA EULA](https://apal-seu.github.io/OPVA/user_agreement.html) |
| **Dataset access** | Email [t.zhang@seu.edu.cn](mailto:t.zhang@seu.edu.cn?subject=OPVA%20Dataset%20Access%20Request) |

## News

| Date | Update |
|------|--------|
| **2026-09** | Project page, user agreement, and annotation splits released. Dataset access is available by signed email request. |
| **2024** | Dataset used in Zhang et al. (IEEE TAC) and Koutsoumpis et al. (Computers in Human Behavior). |

## Overview

OPVA is a facet-activated dataset for personality and job-related competency assessment from asynchronous video interviews. The dataset contains **5,472** interview videos from **684** participants who completed a simulated management traineeship application. Participants answered eight past-behaviour questions, each designed to activate one Extraversion or Conscientiousness facet. OPVA provides HEXACO-60 self-reports, observer-rated Extraversion and Conscientiousness at both factor and facet level, recruiter-rated competencies, demographics, and an official subject-level split.

## Key Features

- **Facet-activated AVI protocol** — 8 personality questions targeting four Extraversion facets and four Conscientiousness facets
- **Psychometrically grounded labels** — HEXACO-60 self-reports and BARS ratings by trained personality raters and professional recruiters
- **Dual assessment targets** — personality traits (X / C factors + eight facets) and job-related competencies in the same interview setting
- **Official split** — subject-level 70 / 10 / 20 (483 / 67 / 134)
- **Academic access** — available after signing the user agreement

## Dataset Statistics

| Property | Value |
|----------|-------|
| Participants | 684 (231 men / 446 women / 7 non-binary) |
| Videos | 5,472 (8 per participant) |
| Age | 31.10 ± 11.53 years |
| Work experience | 11.21 ± 10.52 years |
| Personality labels | HEXACO-60 self-reports + observer Extraversion / Conscientiousness (factor + facet) |
| Competency labels | Development orientation, Communication flexibility, Persuasiveness, Quality orientation, Overall hireability |
| Official split | Subject-level 70 / 10 / 20 (483 / 67 / 134) |

## Files in this repository

This GitHub repository hosts the project page and documentation. Annotation CSVs and interview videos are **not** included here; they are shared after the access request is approved.

| Path | Description |
|------|-------------|
| `CODEBOOK.md` / `CODEBOOK_zh.md` | Column definitions for the annotation release (EN / 中文) |
| `index.html` / `zh.html` | Project page (English / 中文) |
| `user_agreement.html` | End-user license / user agreement |

After access is granted, the data release uses split folders `Training` / `Validation` / `Testing` with annotation CSVs and videos named `{id}_q{1-8}.mp4`.

## Getting Started

1. Read the [User Agreement](https://apal-seu.github.io/OPVA/user_agreement.html).
2. Have a researcher with a permanent position sign the form. Students may be listed as participants.
3. Email the signed PDF to **Tianyi Zhang** at [t.zhang@seu.edu.cn](mailto:t.zhang@seu.edu.cn), with subject `OPVA Dataset Access Request`. Include your name, institution, position, and a brief research statement.

## Citation

If you use OPVA, please cite both papers:

```bibtex
@article{zhang2024llms,
  author  = {Zhang, Tianyi and Koutsoumpis, Antonis and Oostrom, Janneke K. and Holtrop, Djurre and Ghassemi, Sina and de Vries, Reinout E.},
  title   = {Can Large Language Models Assess Personality From Asynchronous Video Interviews? A Comprehensive Evaluation of Validity, Reliability, Fairness, and Rating Patterns},
  journal = {IEEE Transactions on Affective Computing},
  year    = {2024},
  volume  = {15},
  number  = {3},
  pages   = {1769--1785},
  doi     = {10.1109/TAFFC.2024.3374875}
}

@article{koutsoumpis2024beyond,
  author  = {Koutsoumpis, Antonis and Ghassemi, Sina and Oostrom, Janneke K. and Holtrop, Djurre and van Breda, Ward and Zhang, Tianyi and de Vries, Reinout E.},
  title   = {Beyond traditional interviews: Psychometric analysis of asynchronous video interviews for personality and interview performance evaluation using machine learning},
  journal = {Computers in Human Behavior},
  year    = {2024},
  volume  = {154},
  pages   = {108128},
  doi     = {10.1016/j.chb.2023.108128}
}
```

## License

The dataset is released for academic, non-commercial, not-for-profit research. Use of OPVA requires agreeing to the [User Agreement](https://apal-seu.github.io/OPVA/user_agreement.html). Do not redistribute interview videos or attempt to re-identify participants.
