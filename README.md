# Obesity & Snacking ANCOVA

**Statistical inference case study in R examining weight differences across snacking groups while controlling for age**

## Executive Summary
This project uses ANCOVA to compare mean weight across four snacking-frequency groups while adjusting for age. It also estimates adjusted group means and uses a planned contrast to compare the no-snacking group with the average of the three snacking groups.

An important analytical lesson is that a statistically significant **overall factor test** does not imply that every specific contrast is significant.

## Methods Demonstrated
- Data recoding and factor labeling
- Group descriptive statistics
- ANCOVA
- Covariate adjustment
- Estimated marginal means
- Planned contrasts
- Statistical interpretation
- Visualization of a covariate and factor

## Source-Reported Findings
The original coursework reported:
- a statistically significant overall `SNACKS` effect after controlling for age (`p < 2e-16`);
- a non-significant planned “No vs Others” contrast (`p ≈ 0.55`).

These are retained as **coursework-reported findings** because the original Excel dataset was not included in the uploaded repository.

## Why Both Results Can Be True
The overall ANCOVA asks whether there is evidence that at least some adjusted group means differ. The planned contrast asks a narrower question: whether the no-snacking group differs from the average of the other three groups. A significant omnibus test can coexist with a non-significant specific contrast.

## Data Note
The notebook expects `data/Obesity.xlsx`. No new numerical results are claimed until the original data are rerun.

## Interview Talking Point
> I used ANCOVA because I wanted to compare weight across snacking groups while controlling for age. I then used estimated marginal means and a planned contrast to answer a more specific question. The overall snacking factor was significant in the coursework results, but the no-snacking-versus-others contrast was not. That taught me to distinguish an omnibus group effect from a specific hypothesis test.
