---
name: tripod-check
description: Check a prediction model development or validation study against the TRIPOD checklist and say where each item is reported.
---

Use this for a study that develops, validates or updates a multivariable prediction model for diagnosis or prognosis, by regression or by machine learning. For the accuracy of a single test use `stard-check`.

## Get the checklist

1. Obtain the official TRIPOD checklist: a file the collaborator adds to the project, or fetched with fetch_url from the TRIPOD website (www.tripod-statement.org) or the EQUATOR Network (www.equator-network.org). The statement has been updated to cover machine learning methods (TRIPOD+AI replaces the 2015 checklist), so ask which one the journal requires and state which you used. Do not recite items from memory. If the fetch does not return a usable checklist (many are PDF or Word downloads), ask the collaborator to add the file to the project; do not go on from memory.
2. Establish with the collaborator whether the study is development, validation, or both, since items apply differently, and ask whether an extension applies and obtain it too, for example clustered data, systematic reviews of prediction models, large language models, or abstracts.
3. Ask which version and which form the journal requires, and use the guideline's explanation and elaboration document when an item's meaning is unclear.

## Read

4. Read the whole manuscript, every table and figure, and the supplementary files in the project, including any model specification, code or data dictionary.

## Assess

5. For each item, in the checklist's order, record: reported, partly reported, not reported, or not applicable, with the location (section and paragraph, or page and line if the form asks for them) and a brief quotation or the table or figure that supports the judgment. "Partly reported" names what is missing; "not applicable" gives the reason.
6. Judge reporting, not conduct: an item is reported when the manuscript says what was done, including that something was not done. Do not infer a step from usual practice.
7. Pay particular attention to:
   - the source of data, the setting and dates, and the eligibility criteria, separately for development and for each validation set;
   - the outcome: its definition, how and when it was assessed, and whether assessors knew the predictors;
   - every predictor: definition, timing and method of measurement, and all candidates considered, not only those kept;
   - the sample size and the number of outcome events, with how the size was justified;
   - missing data: how much per variable and how it was handled;
   - how continuous predictors were handled, how predictors were selected, and for machine learning methods the tuning procedure and how data were split so that evaluation data did not inform the model;
   - the model is specified fully enough to be used on a new individual (all coefficients and the intercept or baseline, or access to the model and code), with how to obtain a prediction;
   - performance is reported as both calibration and discrimination with precision, with the internal validation method (for example bootstrap or cross-validation) and, for validation, any differences from the development data;
   - participant numbers and outcome events at each stage agree between the text, any flow diagram and the tables;
   - performance across key subgroups where the checklist asks for it, the intended use and users, and limitations including the risk of overfitting. This checks reporting; it is not a risk-of-bias assessment.

## Report

8. Produce the completed checklist as a table in the form the journal asks for, with the official item wording and order, then a short list of gaps, most important first, with the information needed for each, and separately any inconsistency found in step 7.
9. Suggest wording only from what the manuscript or the collaborator provides. Never invent study details such as event counts, coefficients, performance figures, tuning settings or data sources; ask for them and leave a marked placeholder.
10. Edit the manuscript only when asked, and update the locations in the checklist afterwards, since page and line numbers move.
