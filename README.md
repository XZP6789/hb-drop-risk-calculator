# Early Hb Drop ≥30% Risk Calculator

Public web calculator for a locked multilayer perceptron (MLP) model developed to estimate the probability of early hemoglobin decline ≥30% after lumbar fusion.

## Model

- Model version: Strict MLP v1.0
- Predictors: 14
- Network architecture: 14–10–1
- Prespecified decision threshold: 0.0937775 (9.38%)
- Sex coding: Female = 0, Male = 1
- All predictors except sex are standardized using development-set means and standard deviations before prediction.

## Predictors

Sex, operative time, fusion levels, intraoperative fluid, hemoglobin, age, APTT, chloride, albumin, drain count, total protein, RBC count, calcium, and PT.

## Use

The calculator runs entirely in the user's browser. Enter all 14 predictor values and select **Calculate risk**. The page reports the model-predicted probability and whether it is above or below the prespecified operating threshold.

The calculator includes an internal browser-side integrity test using reference cases. Calculation remains disabled if that integrity check fails.

## Important note

This is a research prediction tool. It is intended for research and risk-estimation support and should not replace clinical judgment or be used as a stand-alone treatment decision rule.

## Privacy

The deployed calculator performs prediction locally in the browser and does not require a server-side patient-data submission endpoint.
