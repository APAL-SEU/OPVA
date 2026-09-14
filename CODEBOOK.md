# Column documentation (CSV annotations)

Each row is one participant. Files: `Training.csv` (n=483), `Validation.csv` (n=67), `Testing.csv` (n=134). Total **684**.
HEXACO observer scores and job competencies use a 5-point BARS (1 = very low, 5 = very high; one decimal is allowed). HEXACO-60 self-reports use a 5-point Likert scale (1 = strongly disagree, 5 = strongly agree).

The eight interview questions each activate one Extraversion or Conscientiousness **facet**. Video files are named `{id}_q{1-8}.mp4` and placed under `Training/`, `Validation/`, and `Testing/`.

## Identifiers and demographics

| Column | Meaning | Coding |
| --- | --- | --- |
| `id` | Participant identifier (matches video filenames) | string. Most IDs are 24-character Prolific-style hashes; 40 short IDs (e.g. `OD66`) are snowball-sample participants. |
| `gender` | Self-reported gender | 1 = male; 2 = female; 3 = non-binary / third gender |
| `age` | Age in years | continuous (18–66) |
| `education` | Highest education completed | 1 = less than high school (n=4); 2 = high school graduate (n=55); 3 = lower-than-college / some college (n=183); 4 = college / bachelor or equivalent (n=305); 5 = postgraduate (n=137) |
| `work_experience` | Years of work experience | continuous; **2** training participants missing |
| `job_applications` | Number of jobs applied for in the last two years | count; **2** training participants missing (different IDs from the work-experience gaps) |
| `english_proficiency` | Self-rated English | 1 = well below average … 5 = well above average. Values present: 1, 3, 4, 5 |

## Observer Extraversion / Conscientiousness (`p_*_observer`)

`p_X_observer` / `p_C_observer` are the means of the four corresponding facet columns.

| Column | Meaning | Question | Coding |
| --- | --- | --- | --- |
| `p_X_observer` | Extraversion (observer; mean of four X facets) | q1, q3, q5, q7 | 1–5 |
| `p_C_observer` | Conscientiousness (observer; mean of four C facets) | q2, q4, q6, q8 | 1–5 |
| `p_Xsses_observer` | Social self-esteem | q1 | 1–5 |
| `p_Xsbol_observer` | Social boldness | q3 | 1–5 |
| `p_Xsoci_observer` | Sociability | q5 | 1–5 |
| `p_Xlive_observer` | Liveliness | q7 | 1–5 |
| `p_Corga_observer` | Organization | q2 | 1–5 |
| `p_Cdili_observer` | Diligence | q4 | 1–5 |
| `p_Cperf_observer` | Perfectionism | q6 | 1–5 |
| `p_Cprud_observer` | Prudence | q8 | 1–5 |

## Self-report HEXACO (`*_self`)

HEXACO-60: 10 items per domain; domain score = mean of the 10 (reverse-keyed) items.

| Column | Meaning | Coding |
| --- | --- | --- |
| `H_self` | Honesty-Humility (self) | 1–5 |
| `E_self` | Emotionality (self) | 1–5 |
| `X_self` | Extraversion (self) | 1–5 |
| `A_self` | Agreeableness (self) | 1–5 |
| `C_self` | Conscientiousness (self) | 1–5 |
| `O_self` | Openness to Experience (self) | 1–5 |

## Observer job competencies (`mean_rating_*`)

Mean of two professional recruiters.

| Column | Meaning | Coding |
| --- | --- | --- |
| `mean_rating_dev_orient` | Development orientation: effort to broaden skills and grow professionally | 1–5 |
| `mean_rating_com_flex` | Communication flexibility: convey a message in different ways depending on the audience | 1–5 |
| `mean_rating_persuasiveness` | Persuasiveness: gain agreement through arguments, authority, and/or diplomacy | 1–5 |
| `mean_rating_qual_orient` | Quality orientation: effort to meet or exceed quality standards | 1–5 |
| `mean_rating_hirea` | Overall hireability for the management-traineeship role | 1–5 |

## Split

| Split | n | Annotation file | Video folder |
| --- | --- | --- | --- |
| train | 483 | `Training.csv` | `Training/` |
| validation | 67 | `Validation.csv` | `Validation/` |
| test | 134 | `Testing.csv` | `Testing/` |
