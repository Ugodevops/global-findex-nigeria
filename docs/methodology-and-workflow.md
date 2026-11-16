# Methodology and Project Workflow

## 1. Project background

Financial inclusion increasingly involves both access to financial services and the digital channels through which people access or use them. Mobile phone ownership and internet use may be relevant to these patterns, but their relationship with financial inclusion should be investigated rather than assumed.

This project uses the World Bank's Global Findex Database 2025 to examine these relationships in Nigeria.

## 2. Objective and research questions

**Objective**

Use data to understand how access to and use of digital technology relate to people's access to and use of financial services in Nigeria.

The objective was translated into five questions:

1. What are the patterns of mobile phone ownership and internet use?
2. How does internet use relate to financial institution accounts, mobile money accounts and digital payments?
3. How does financial inclusion vary by age, and what patterns emerge when digital technology use is considered?
4. How do digital technology and financial inclusion differ by gender?
5. How do digital technology and financial inclusion differ between rural and urban respondents?

The questions determine which indicators and comparison groups are relevant. They also define the limits of what the project can claim.

## 3. Data source and scope

- **Source:** World Bank, Global Findex Database 2025.
- **Working workbook:** `findex_microdata_2025_labelled_update112425.xlsx`.
- **Geographic focus:** Nigeria.
- **Data type:** Individual-level survey microdata.
- **Unit of analysis:** Survey respondent / individual.
- **Source documentation:** World Bank Global Findex materials, questionnaire and microdata documentation.

The original source workbook contains multiple sheets and country records. The analysis focused on the Nigeria records. The source microdata are not committed to this repository; users should obtain them from the World Bank and respect the applicable access and use conditions.

## 4. Indicator framework

| Analytical dimension | Indicator | Analytical use |
|---|---|---|
| Digital technology | Mobile phone ownership | Compare internet use by phone-ownership category |
| Digital technology | Internet use | Compare financial inclusion across the reported internet-use categories |
| Financial inclusion | Financial institution account ownership | Measure access to an account at a financial institution |
| Financial inclusion | Mobile money account ownership | Examine mobile money account ownership |
| Financial inclusion | Digital payment participation | Examine participation in digital payments |
| Demographic | Age | Compare financial inclusion across age groups |
| Demographic | Gender | Compare reported financial inclusion indicators between male and female respondents |
| Geographic | Urban/rural residence | Compare reported financial inclusion indicators by residence |

The project used the labels and definitions available in the source materials and report. Exact variable definitions, response codes and denominator rules should always be checked against the official questionnaire and data dictionary before reproducing the measures.

## 5. Data inspection and quality assessment

The workbook was inspected before analysis. The work included:

- Reviewing the workbook sheets and the structure of the labelled data.
- Examining variable names, data types, distinct values and missingness.
- Profiling columns to distinguish valid values, errors and empty values.
- Checking categories that represent substantive responses, including No, Don't know and Refused.
- Identifying the need to keep missing/empty values distinct from explicit survey responses.

This distinction matters. An empty value does not necessarily mean No. Similarly, Don't know and Refused are response categories, not ordinary missing values, and should not be silently recoded as No.

The project used Power Query for workbook inspection and quality profiling, with Python used for selected exploratory checks.

## 6. Data preparation

The analysis focused on the Nigeria records and the variables relevant to the five research questions. Preparation and analytical checks included reviewing the categories used for age, gender, internet use, mobile phone ownership and urban/rural residence.

Examples of fields examined during the project included:

- `economy` — country/economy identifier.
- `age` — respondent age.
- `internet_use` — internet-use indicator.
- `con1` — mobile phone ownership response.
- `educ` — education category.
- `account_fin` — financial institution account indicator.
- `account_mob` — mobile money account indicator.
- `merchantpay_dig`, `anydigpayment` and `nydigpayment` — digital-payment-related fields examined during exploration.
- `urbanicity` — urban/rural residence category.

This list is an analytical working guide, not a substitute for the official data dictionary. The full field names, labels, universes and response codes must be checked in the source documentation.

## 7. Analysis and visualisation

Power BI was used to compare the indicators across relevant groups. The report included comparisons such as:

- Internet use by mobile phone ownership.
- Financial inclusion indicators by internet-use category.
- Financial inclusion indicators across age groups.
- Financial inclusion indicators by gender.
- Financial inclusion indicators by urban/rural residence.

The analysis was descriptive and comparative. Percentages were used to make differences between groups easier to interpret. Where a visual used weighted percentages, the figures were documented as weighted percentages. The mobile-phone/internet comparison was documented as unweighted.

A percentage must always be interpreted with its denominator, response category, weighting status and survey universe in mind. A difference between two percentages is a descriptive gap, not proof of a causal effect.

## 8. Interpretation and reporting

The reporting process moved from values to observations and then to cautious interpretation:

1. State the values shown in the visual.
2. Identify which group has the higher or lower reported percentage.
3. Calculate or state the percentage-point difference where the figures are available.
4. Explain what the pattern may suggest without claiming that it proves a cause.
5. State what the visual does not show.
6. Record recommendations as areas for consideration or further investigation, not as effects proven by the analysis.

## 9. Limitations

- The mobile phone ownership/internet use comparison is unweighted, unlike the weighted comparisons reported in other sections.
- The No/DK/Refused category is retained as displayed and cannot be treated as a confirmed non-internet-use category.
- The age visual does not show the requested age-by-internet-use comparison.
- The gender visual does not show gender comparisons for mobile phone ownership or internet use.
- The rural/urban visual does not show geographical comparisons for mobile phone ownership or internet use.
- A verified mobile-money result for the internet-use comparison was not retained in the final project record and is therefore not reported here.
- The exact survey sample design, weights, indicator denominators and eligibility universes should be consulted in the official documentation before making population-level claims.
- Descriptive comparisons do not establish causation.

## 10. Reproducibility

To reproduce or extend the work:

1. Download the Global Findex 2025 data and associated documentation from the World Bank.
2. Confirm the version of the data file and questionnaire.
3. Identify Nigeria records using the official country/economy field.
4. Confirm variable labels, response codes, missing-value conventions and indicator universes.
5. Recreate the data preparation and Power BI measures.
6. Verify whether each reported visual uses weighted or unweighted percentages.
7. Check denominators and compare recreated outputs against the values documented in the findings file.

The original microdata are not included in this repository. Reproduction requires the source data and documentation.
