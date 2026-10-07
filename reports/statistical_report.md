# Statistical Validation Report

## Purpose

This report records the statistical validation performed in Step 4. Each tested finding is documented with the claim, statistical test, result, effect size where applicable, sample size, and a plain-English verdict.

## T1. Does winning the toss help you win the match?

### Claim
Winning the toss helps a team win the match.

### Hypothesis
- **H₀:** The toss winner's true match-win rate is 50%.
- **H₁:** The toss winner's true match-win rate is different from 50%.

### Test
Binomial test.

### Result
- Decisive matches: **1,187**
- Toss winner also won: **613**
- Observed win rate: **51.64%**
- p-value: **0.2700**
- 95% Wilson confidence interval: **48.80%–54.48%**
- Effect: **1.64 percentage points above 50%**

### Verdict
**NOT SIGNIFICANT.**

The p-value is greater than 0.05, so we fail to reject H₀. There is insufficient evidence that winning the toss changes the chance of winning the match.

---

## T2. Does the decision taken after the toss matter?

### Claim
The decision made after winning the toss is associated with match outcome.

### Hypothesis
- **H₀:** Batting first and fielding first have the same win rate.
- **H₁:** Their win rates are different.

### Test
Chi-square test of independence.

### Result
- Bat first: **184 wins, 218 losses**
- Bat-first win rate: **45.77%**
- Field first: **429 wins, 356 losses**
- Field-first win rate: **54.65%**
- Difference: **8.88 percentage points**
- Chi-square: **8.04**
- p-value: **0.0046**
- Degrees of freedom: **1**

### Verdict
**SIGNIFICANT.**

The p-value is less than 0.05, so we reject H₀. The decision taken after the toss is associated with match outcome. The guide notes that this is another view of the chase advantage tested in T3, rather than a completely separate effect.

---

## T3. Does the chasing team have an advantage?

### Claim
The chasing team has an advantage.

### Hypothesis
- **H₀:** The chase win rate is 50%.
- **H₁:** The chase win rate is different from 50%.

### Test
Binomial test.

### Result
- Decisive matches: **1,187**
- Successful chases: **647**
- Chase win rate: **54.51%**
- Difference from 50%: **4.51 percentage points**
- p-value: **0.0021**
- 95% Wilson confidence interval: **51.66%–57.32%**

### Verdict
**SIGNIFICANT.**

The p-value is less than 0.05, so we reject H₀. There is evidence that the chase win rate differs from 50%, with the observed rate being above 50%.


## T4. Does chase win rate fall as the target rises?

### Claim
The chance of winning a chase decreases as the target becomes larger.

### Hypothesis
- **H₀:** Chase win rates are the same across target bands.
- **H₁:** Chase win rates are not the same across target bands.

### Test
Chi-square test of independence.

### Result
- Target bands: **5**
- Highest chase win rate: **82.6%** for targets under 140
- Lowest chase win rate: **23.2%** for targets of 200+
- Difference: **approximately 59 percentage points**
- Chi-square: **197.68**
- Degrees of freedom: **4**
- p-value: **approximately 1 × 10⁻⁴¹**

### Verdict
**SIGNIFICANT.**

The p-value is far below 0.05, so we reject H₀. Chase outcome is strongly associated with target band, with much lower chase success at higher targets.

---

## T5. Are defended totals actually bigger than chased ones?

### Claim
Teams that defend a total score more in the first innings, on average, than teams whose target is successfully chased.

### Hypothesis
- **H₀:** The mean first-innings scores of the two groups are equal.
- **H₁:** The mean first-innings scores are different.

### Test
Independent two-sample t-test with unequal variances.

### Result
- Defended matches: **540**
- Successful chase matches: **647**
- Defended average: **183.3 runs**
- Chased average: **155.5 runs**
- Difference: **27.8 runs**
- t-statistic: **15.73**
- p-value: **1.17 × 10⁻⁵⁰**
- Cohen's *d*: **0.92**
- Effect-size interpretation: **Large**

### Verdict
**SIGNIFICANT, AND LARGE.**

The p-value is far below 0.05, so we reject H₀. The average first-innings score is substantially higher in defended matches, and the effect size is large.

---

## T6. Is powerplay really faster than middle overs?

### Claim
Teams score faster during the powerplay than during the middle overs.

### Hypothesis
- **H₀:** Powerplay and middle-over scoring rates are the same.
- **H₁:** The two scoring rates are different.

### Test
Paired t-test.

### Result
- Valid innings: **2,406**
- Powerplay average: **8.02 runs/over**
- Middle-over average: **7.95 runs/over**
- Difference: **approximately 0.08 runs/over**
- t-statistic: **1.53**
- p-value: **0.1259**

### Verdict
**NOT SIGNIFICANT.**

The p-value is greater than 0.05, so we fail to reject H₀. There is insufficient evidence of a measurable difference between powerplay and middle-over scoring rates in this test. Therefore, the Step 3 finding that powerplay is faster does not hold statistically.

---

## T7. Do left-handers really hit harder than right-handers?

### Claim
Left-handed batters have a higher strike rate than right-handed batters.

### Hypothesis
- **H₀:** Left-handed and right-handed batters have the same average strike rate.
- **H₁:** Their average strike rates are different.

### Test
Independent two-sample t-test with unequal variances.

### Result
- Total batters: **137**
- Left-handed batters: **50**
- Right-handed batters: **87**
- Left-handed average strike rate: **136.60**
- Right-handed average strike rate: **136.62**
- Difference: **-0.02**
- p-value: **0.9942**
- Cohen's *d*: **0.001**
- Effect-size interpretation: **Essentially zero**

### Verdict
**NOT SIGNIFICANT, WITH ESSENTIALLY ZERO EFFECT.**

The p-value is greater than 0.05, so we fail to reject H₀. There is insufficient evidence that left-handed and right-handed batters have different average strike rates. The effect size is essentially zero.
0, ,0
