

## 1. Levels (Scales) of Measurement

| **Scale**    | **Properties**                                                                                     | **Permissible Statistics**             | **Key Feature**           |
| ------------ | -------------------------------------------------------------------------------------------------- | -------------------------------------- | ------------------------- |
| **Nominal**  | • Identity only: each value names or labels a category<br>• No order, no distance                  | Mode only                              | Classification            |
| **Ordinal**  | • Identity + Order: values can be ranked<br>• No assumption of equal intervals                     | Median, percentiles, mode              | Ranking                   |
| **Interval** | • Identity + Order + Equal intervals: differences meaningful<br>• No true zero (arbitrary zero)    | Mean, standard deviation, correlations | Differences but no ratios |
| **Ratio**    | • Identity + Order + Equal intervals + True zero: zero means “none”<br>• All arithmetic operations | All (mean, SD, ratios, geometric mean) | Full numeric operations   |

---

## 2. Nominal Scale

* **Definition:**
  Variables whose values are names or labels for distinct categories. There is no logical order.

* **Characteristics:**

  * Categories are mutually exclusive and exhaustive.
  * You can only test equality (“= / ≠”).

* **Permissible Analyses:**

  * Frequency counts, proportions, chi-square tests.
  * Mode.

* **Examples:**

  * **Demographics:** Gender (Male, Female, Other), Blood type (A, B, AB, O), Marital status (Single, Married, Divorced).
  * **Marketing:** Product ID codes, Brand names, Zip codes.
  * **Medical:** Presence/absence of disease (Yes/No), Eye color (Blue, Brown, Green).

---

## 3. Ordinal Scale

* **Definition:**
  Categories that can be **ranked**, but intervals between ranks are not equal or known.

* **Characteristics:**

  * Allows order comparisons (“> / <”).
  * Cannot meaningfully add or subtract.

* **Permissible Analyses:**

  * Median, percentiles, non-parametric tests (e.g. Mann–Whitney U, Wilcoxon).
  * Mode.

* **Examples:**

  * **Surveys:** Likert items (“Strongly disagree” → “Strongly agree”), satisfaction ratings (1–5 stars).
  * **Education:** Letter grades (A > B > C), class rank (1st, 2nd, 3rd).
  * **Health:** Pain scale (No pain, Mild, Moderate, Severe), cancer staging (Stage I, II, III, IV).

---

## 4. Interval Scale

* **Definition:**
  Ordered categories with **equal intervals** between values, but an **arbitrary zero**.

* **Characteristics:**

  * Differences are meaningful (e.g. difference between 20 and 30 is same as 80 and 90).
  * Ratios are **not** meaningful because zero is not “absence” (e.g. 20°C is not “twice as hot” as 10°C).

* **Permissible Analyses:**

  * All arithmetic except true ratios: mean, standard deviation, correlation, regression.

* **Examples:**

  * **Temperature:** Celsius, Fahrenheit.
  * **Psychometrics:** IQ scores (mean 100, SD 15).
  * **Calendar:** Years on the Common Era scale (e.g. 2000 vs. 1500).
  * **Finance:** Credit scores (e.g. 300–850 scale).

---

## 5. Ratio Scale

* **Definition:**
  All properties of interval scales **plus** a **true zero** that indicates absence of the attribute.

* **Characteristics:**

  * Zero means “none” (e.g. zero weight means nothing weighs).
  * Both differences and ratios are meaningful (e.g. 4 kg is twice 2 kg).

* **Permissible Analyses:**

  * All arithmetic operations: mean, SD, geometric mean, coefficient of variation, ratios.

* **Examples:**

  * **Physical Measures:** Height (cm), weight (kg), distance (m).
  * **Time:** Duration (seconds), age (years since birth).
  * **Counts:** Number of accidents, number of children.
  * **Economics:** Income (dollars), expenditure, population size.

---

## 6. More Examples by Domain

| **Domain**     | **Nominal**                             | **Ordinal**                          | **Interval**                      | **Ratio**                          |
| -------------- | --------------------------------------- | ------------------------------------ | --------------------------------- | ---------------------------------- |
| **Medicine**   | Blood group (A/B/AB/O)                  | Stages of disease (I–IV)             | Body temperature (°C)             | Serum cholesterol (mg/dL)          |
| **Education**  | Major subject (Math, History, Biology)  | GPA letter grade (A, B, C…)          | Standardized test T-scores        | Number of credits earned           |
| **Sports**     | Team names (Lions, Tigers)              | Tournament placement (1st, 2nd, 3rd) | Golf handicap index               | Race time (minutes, seconds)       |
| **Business**   | Industry sector (Tech, Retail, Finance) | Customer satisfaction (1–5 scale)    | Net Promoter Score (–100 to +100) | Sales revenue (USD)                |
| **Psychology** | Personality type (A/B/C…)               | Rank order of preferences            | SAT score                         | Reaction time (ms)                 |
| **Geography**  | Country names                           | Development level (Low, Med, High)   | Longitude/latitude (degrees)      | Elevation above sea level (meters) |

---

### 7. Practical Tips for Choosing the Right Scale

1. **Ask:** What does “zero” represent?

   * If zero means “none,” you likely have a **ratio** scale.
   * If zero is arbitrary, it’s **interval**.

2. **Check Order & Distance:**

   * Can you rank? Yes → at least **ordinal**.
   * Are intervals equal? Yes → at least **interval**.

3. **Statistical Methods Depend on Scale:**

   * Nominal → non-parametric, chi-square.
   * Ordinal → medians, rank tests.
   * Interval/Ratio → means, correlations, regressions.

