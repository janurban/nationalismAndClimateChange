Surprising statistics about Czechia and national attachment (pilot 2)
================
19 listopadu 2026

- [Design](#design)
- [Sample](#sample)
- [Scoring](#scoring)
- [Table 1. Estimates, correct answers and
  surprise](#table-1-estimates-correct-answers-and-surprise)
- [Table 2. Before vs. after the
  manipulation](#table-2-before-vs-after-the-manipulation)
  - [Robustness checks](#robustness-checks)
- [Notes](#notes)

## Design

Participants were randomly assigned (`groupno = rand(1,2)`) to complete
two batteries, **national pride** (6 items, 4-point) and **nationalism**
(4 items, 5-point), either **before** (group 1) or **after** (group 2)
seven trials. In each trial they estimated Czechia’s rank on a
statistic, were shown the true (flattering) rank, and rated how
surprising it was (1 = not at all, 5 = very surprising). The design is
between-subjects.

## Sample

Of 331 started responses, 265 were completed. After the exclusions set
in the YAML parameters (completed only: TRUE; Czech citizens only: TRUE;
repeat participants removed: TRUE), the analysed sample is **N = 263**
(before: n = 124; after: n = 139).

| Condition           |   n | Age M (SD)  | % women |
|:--------------------|----:|:------------|:--------|
| Before manipulation | 124 | 31.9 (11.6) | 67      |
| After manipulation  | 139 | 30.5 (9.6)  | 57      |

Sample by condition

## Scoring

Pride items (A1 = very proud … A4 = not at all proud) were recoded to
1–4 and nationalism items (A1 = strongly agree … A5 = strongly disagree)
to 1–5, so that higher values mean more pride or nationalism. Scale
scores are item means.

| Battery     | Before manipulation | After manipulation | Total |
|:------------|--------------------:|-------------------:|------:|
| Pride       |                0.67 |               0.62 |  0.65 |
| Nationalism |                0.56 |               0.58 |  0.58 |

Cronbach’s alpha

## Table 1. Estimates, correct answers and surprise

| Statistic | Range | Correct rank | n | Estimate M (SD) | Estimate Mdn | % placed CZ lower | % exact | Surprise M (SD) |
|:---|:---|---:|---:|---:|---:|---:|---:|---:|
| Lowest unemployment in the EU | 1–27 | 1 | 262 | 4.34 (4.30) | 3 | 81 | 19 | 2.30 (1.39) |
| GDP per capita among 30 post-communist countries | 1–30 | 2 | 263 | 4.80 (5.47) | 3 | 57 | 23 | 2.08 (1.31) |
| Number of castles/chateaux among 50 European countries | 1–50 | 1 | 261 | 6.98 (8.99) | 4 | 83 | 17 | 2.57 (1.49) |
| Subjective happiness among 160+ countries | 1–160 | 20 | 259 | 41.82 (32.01) | 31 | 68 | 6 | 2.84 (1.29) |
| Overall sustainability among 160+ countries | 1–160 | 12 | 259 | 33.55 (28.95) | 25 | 81 | 2 | 3.10 (1.39) |
| Age of Charles University among CEE universities | 1–100 | 1 | 262 | 7.23 (17.67) | 2 | 59 | 41 | 1.73 (1.09) |
| Public libraries per capita among 160+ countries | 1–160 | 1 | 263 | 16.62 (24.85) | 10 | 84 | 16 | 2.94 (1.52) |

Estimated rank of Czechia vs. the correct rank (1 = best). Surprise: 1 =
not at all, 5 = very surprising.

Respondents placed Czechia lower than its actual rank on every
statistic. The share who did so ranged from 57% to 84%. Average surprise
across the seven trials was *M* = 2.51 (*SD* = 0.83). The most
surprising fact was “Overall sustainability among 160+ countries” (*M* =
3.10) and the least surprising was “Age of Charles University among CEE
universities” (*M* = 1.73).

Rank estimates are right-skewed, so medians are reported alongside
means.

## Table 2. Before vs. after the manipulation

| Measure | Before M (SD) | After M (SD) | t (df) | p | d \[95% CI\] |
|:---|:--:|:--:|:--:|:--:|:--:|
| National pride (1–4) | 2.83 (0.45) | 2.96 (0.45) | 2.30 (258.2) | 0.022 | 0.28 \[0.04, 0.53\] |
| Nationalism (1–5) | 3.03 (0.69) | 3.25 (0.69) | 2.62 (257.6) | 0.009 | 0.32 \[0.08, 0.57\] |

Welch two-sample t-tests (between-subjects). Positive t and d mean
higher scores after the surprising statistics.

- **National pride (1–4):** before *M* = 2.83 (*SD* = 0.45, *n* = 124),
  after *M* = 2.96 (*SD* = 0.45, *n* = 139); *t*(258.2) = 2.30, *p* =
  .022, *d* = 0.28, 95% CI \[0.04, 0.53\].
- **Nationalism (1–5):** before *M* = 3.03 (*SD* = 0.69, *n* = 124),
  after *M* = 3.25 (*SD* = 0.69, *n* = 139); *t*(257.6) = 2.62, *p* =
  .009, *d* = 0.32, 95% CI \[0.08, 0.57\].

### Robustness checks

| Measure              | Student t (df) | Student p | Mann–Whitney W | Mann–Whitney p |
|:---------------------|:---------------|:----------|:---------------|:---------------|
| National pride (1–4) | 2.30 (261)     | 0.022     | 10031          | 0.021          |
| Nationalism (1–5)    | 2.62 (261)     | 0.009     | 10163          | 0.012          |

Equal-variance t-test and Mann–Whitney U test

<figure>
<img src="surprising_statistics_report_files/figure-gfm/plot-1.png"
alt="Scale scores by condition (means ± 95% CI)." />
<figcaption aria-hidden="true">Scale scores by condition (means ± 95%
CI).</figcaption>
</figure>

## Notes

- The data are the LimeSurvey coded export, downloaded from
  <https://raw.githubusercontent.com/janurban/nationalismAndClimateChange/main/data_coded.xlsx>.
  Correct ranks are taken from the feedback shown to respondents.
- Internal consistency is modest (see the reliability table), so treat
  the scale-level effects with caution.
- Sample exclusions are controlled by the YAML `params` and can be
  changed without editing the code, e.g.
  `rmarkdown::render("surprising_statistics_report.Rmd", params = list(drop_repeated = FALSE))`.
