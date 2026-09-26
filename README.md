# Companion data — pre-treatment TB loss to follow-up, West Java

Aggregate results, tables and figures accompanying the article:

> **Spatial transferability of explainable machine learning for predicting pre-treatment
> tuberculosis loss to follow-up across districts and cities in West Java, Indonesia**
> *BMC Medical Informatics and Decision Making*

**Live page:** https://rdwnilyas-coder.github.io/tb-ptlfu-westjava-companion/

## What is here

| Path | Contents |
|---|---|
| `index.html` | The companion page: every aggregate table and figure from the article |
| `data/companion.json` | All numbers on the page, in one machine-readable file |
| `figs/` | Every figure in the article, at submission resolution |

The page covers:

- **Predictor value details** — for each predictor, the number of patients, observed loss rate,
  and adjusted odds ratio with confidence interval for every category. The article reports
  predictor importance and refers the reader here for the value-level detail.
- **Transferability by district and city** — leave-one-district-out AUC, bootstrap confidence
  interval, observed and predicted rates, calibration gap, and the distribution of key predictors.
- **Adjusted odds ratios by area** from the development model.
- **Model comparison and calibration** — five algorithms, each with and without balanced class
  weights, reported against a prevalence-based baseline Brier score.
- **Effect of local recalibration**, evaluated out of fold within each area.
- **Integer risk scorecard**, with every level listed and tier rates under three validation schemes.
- **Spatial statistics** under three neighbourhood definitions.
- **Feature selection** across three strategies, and the within-fold selection check.
- **Learning curve** for the linear model and the best-performing ensemble.
- **Reproducibility specification** — library versions, seed, folds, subsample sizes.

## What is not here

**No individual patient record is published in this repository, and no variable that could
identify a patient.** The smallest unit reported is an entire district or city; the smallest
such unit contains 709 cases.

Individual-level surveillance records come from the Indonesian national Tuberculosis Information
System (Sistem Informasi Tuberkulosis, SITB), managed by the Ministry of Health of the Republic
of Indonesia, and were made available for this study by the Provincial Health Office of West Java.
They contain identifiable information and cannot be deposited publicly under the terms of the
institutional permission granted. Requests for access may be directed to the corresponding author
and are subject to approval by the Provincial Health Office of West Java.

## Study at a glance

- 174,201 tuberculosis cases diagnosed in West Java Province, registered 1 January – 30 September 2024
- Register cut-off 29 September 2025, giving 364 to 637 days of follow-up per patient
- Pre-treatment loss to follow-up: 9.13 percent
- 27 districts and cities

## Ethics

Approved by the Health Research Ethics Committee of Universitas Islam Bandung,
No. 217/KEPK-Unisba/XII/2025.

## Contact

Ridwan Ilyas — ilyas@lecture.unjani.ac.id
