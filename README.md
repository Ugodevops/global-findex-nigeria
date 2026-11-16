# Global Findex Nigeria: Digital Technology and Financial Inclusion

[![Portfolio project](https://img.shields.io/badge/Portfolio-Economy%20%7C%20E1-blue)](https://github.com/Ugodevops/development-research-data-portfolio)

## Dashboard preview

![Global Findex Nigeria Power BI dashboard](images/Screenshot%202026-11-16%20113528.png)

*Power BI report overview: digital access and financial inclusion indicators across internet-use categories, age groups, gender and residential location.*

## Project overview

This project uses the World Bank's Global Findex Database 2025 to explore how access to and use of digital technology relate to people's access to and use of financial services in Nigeria.

The work follows a research-to-reporting workflow: defining the problem, setting an objective, developing analytical questions, inspecting and preparing the data, comparing indicators in Power BI, interpreting results, and documenting limitations.

**Project objective**

> Use data to understand how access to and use of digital technology relate to people's access to and use of financial services in Nigeria.

**Project type:** National survey microdata analysis  
**Geographic focus:** Nigeria  
**Portfolio classification:** Economy — E1  
**Primary deliverable:** Power BI report  
**Analysis type:** Descriptive and comparative; not a causal-impact study

## Research questions

1. **Digital access:** What are the patterns of access to and use of digital technology among individuals in Nigeria, particularly in relation to mobile phone ownership and internet use?
2. **Digital technology and financial inclusion:** How does internet use relate to individuals' access to and use of financial services, particularly financial institution accounts, mobile money accounts and digital payments?
3. **Age and financial inclusion:** How do access to and use of financial services vary across different age groups, and what patterns emerge when digital technology use is considered?
4. **Gender and financial inclusion:** How do access to and use of digital technology and financial services differ between male and female respondents?
5. **Geographical differences:** How do access to and use of digital technology and financial services differ between individuals living in rural and urban areas of Nigeria?

## Analytical framework

| Dimension | Indicators used in the project |
|---|---|
| Digital technology | Mobile phone ownership; internet use |
| Financial inclusion | Financial institution account ownership; mobile money account ownership; digital payment participation |
| Demographic context | Age; gender |
| Geographic context | Rural/urban residence |

The project examines differences and associations across these dimensions. A relationship observed in descriptive data is not, by itself, evidence that one factor causes another.

## Data source

**World Bank — Global Findex Database 2025**

The source provides survey microdata and documentation on account ownership, digital payments, mobile money, internet use and related financial inclusion topics.

- [Global Findex](https://www.worldbank.org/en/publication/globalfindex)
- [World Bank Microdata Library](https://microdata.worldbank.org/)

The working source workbook used during the project was named `findex_microdata_2025_labelled_update112425.xlsx`. The source data are not redistributed in this repository. Users should obtain the data and accompanying documentation from the World Bank and follow the applicable terms of use.

## Tools and technologies

- **Excel / Power Query:** workbook inspection, data profiling, quality checks and preparation.
- **SQL (PostgreSQL):** querying and examining the prepared Nigeria dataset, practising analytical filtering, grouping and aggregation, and checking patterns in the data.
- **Python:** exploratory data inspection and selected checks during the analysis.
- **Power BI:** comparative visuals and the final interactive report.
- **DAX / Power BI measures:** calculations used in the report, where applicable.
- **GitHub:** project documentation and versioned deliverables.

## Project workflow

1. Define the development issue and the analytical objective.
2. Translate the objective into five answerable research questions.
3. Identify the indicators and demographic/geographic dimensions relevant to each question.
4. Inspect the Global Findex workbook, its sheets, fields, categories and missing values.
5. Assess data quality, distinguishing empty values from substantive response categories such as No, Don't know and Refused.
6. Prepare and filter the data for the Nigeria analysis.
7. Compare digital access and financial inclusion indicators in Power BI.
8. Interpret the observed patterns without making unsupported causal claims.
9. Document findings, recommendations, assumptions and limitations.
10. Publish the report and supporting documentation.

A fuller account of the workflow and analytical decisions is available in [Methodology and workflow](docs/methodology-and-workflow.md).

## Selected findings

The completed Power BI analysis reported the following patterns:

- In the mobile-phone comparison, internet use was 58.91% among mobile phone owners and 12.50% among respondents without a mobile phone. This comparison is an **unweighted** result.
- In the weighted internet-use comparison, financial institution account ownership was 86.17% in the internet-use category and 43.38% in the No/DK/Refused category. Digital payment participation was 83.42% and 36.94%, respectively.
- Across the reported age groups, respondents aged 31–40 had the highest financial institution account ownership (75.41%); respondents aged 21–30 had the highest digital payment participation (65.86%) and mobile money account ownership (43.22%).
- Male respondents recorded higher percentages than female respondents across the three reported financial inclusion indicators.
- Urban respondents recorded higher percentages than rural respondents across the three reported financial inclusion indicators.

The complete figures, comparisons and reservations are in [Findings and interpretation](docs/findings-and-interpretation.md).

## Important limitations

- The mobile-phone/internet comparison is unweighted, while the other reported comparisons use weighted percentages. They should not be treated as directly interchangeable.
- The No/DK/Refused category retains the classification shown in the report; it should not be interpreted as a pure group of confirmed non-internet users.
- The available age visual does not include the age-by-internet-use comparison.
- The available gender visual does not provide direct male/female comparisons for mobile phone ownership or internet use.
- The available rural/urban visual does not provide direct geographical comparisons for mobile phone ownership or internet use.
- A mobile-money percentage for the internet-use comparison is not included in this repository's findings because a verified figure was not available in the retained project record.
- The analysis is descriptive. It does not establish causation.
- The exact sample design, weighting procedure, and indicator denominators should be checked against the official survey documentation before interpreting the reported percentages as population estimates.

## Repository contents

```text
global-findex-nigeria/
├── README.md
├── Global_findex_Nigeria.pbix
├── images/
│   └── Screenshot 2026-11-16 113528.png
└── docs/
    ├── methodology-and-workflow.md
    ├── findings-and-interpretation.md
    └── variable-guide.md
```

## Reproducing or extending the analysis

1. Obtain the Global Findex 2025 data and documentation from the World Bank.
2. Review the questionnaire and data dictionary before assigning meanings to codes.
3. Filter the source data to Nigeria and verify the resulting records and categories.
4. Recreate the preparation and indicator definitions documented in this repository.
5. Open the Power BI file to inspect the report visuals and measures.
6. Validate weighting, denominators, missing-value treatment and indicator definitions before reproducing or extending the reported percentages.

The source microdata are not included. Reproduction therefore requires obtaining the original dataset and applying the documented source and indicator definitions.

## Portfolio link

This project is part of the [Development Research & Data Intelligence Portfolio](https://github.com/Ugodevops/development-research-data-portfolio), under the **Economy** pillar.

## Author

Umeh Ugochukwu

---
*This repository documents an applied survey-data analysis project. Findings are presented with their methodological limitations and should not be interpreted as causal evidence.*
