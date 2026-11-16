# Variable Guide and Indicator Framework

## Purpose

This guide lists selected fields examined during the Global Findex Nigeria project. It is a practical orientation document, not a replacement for the official World Bank questionnaire or data dictionary.

Always verify variable labels, response codes, question universe, skip patterns and indicator construction against the exact source-file version before reproducing a result.

## Selected fields examined

| Field name | Working description in the project | Use |
|---|---|---|
| `economy` | Country/economy identifier | Select Nigeria records |
| `age` | Respondent age | Age-group comparisons |
| `internet_use` | Internet-use indicator | Digital access and financial inclusion comparisons |
| `con1` | Mobile phone ownership response | Compare internet use by phone ownership |
| `educ` | Education category | Exploratory subgroup analysis |
| `account_fin` | Financial institution account indicator | Financial inclusion |
| `account_mob` | Mobile money account indicator | Financial inclusion |
| `merchantpay_dig` | Digital merchant-payment-related indicator | Digital payment exploration |
| `anydigpayment` | Digital payment indicator examined in exploration | Digital payment analysis |
| `nydigpayment` | Digital payment-related field examined in exploration | Supporting analysis |
| `urbanicity` | Urban/rural residence category | Geographical comparisons |

## Selected category notes recorded during analysis

The following coding notes were observed during the project and must still be checked against the exact questionnaire and data dictionary before reuse:

- `educ`: 1 = primary or less; 2 = secondary; 3 = tertiary or above.
- `urbanicity`: 1 = rural; 2 = urban.
- `con1`: 1 = yes; 2 = no; 3 = don't know; 4 = refused.
- `internet_use`: values 0 and 1 were examined. Confirm the official value labels before assigning meanings in a new analysis.

## Indicator distinctions

**Financial institution account ownership** and **mobile money account ownership** are separate indicators. They should not be combined or treated as interchangeable.

**Digital payment participation** measures an activity, whereas account ownership measures access/ownership. A respondent may have an account without participating in every digital payment activity.

**Internet use** and **mobile phone ownership** are also distinct. Phone ownership does not automatically mean that a respondent uses the internet.

## Missing values and survey responses

Keep these concepts separate:

- **Empty / missing:** no recorded value in the relevant field.
- **No:** an explicit negative response.
- **Don't know:** a substantive survey response category.
- **Refused:** a substantive survey response category.

Do not automatically convert Don't know, Refused or empty values into No. Check the question universe and skip patterns before calculating percentages.

## Recommended checks before building a measure

For every indicator, record:

1. Exact source variable or derived definition.
2. Question wording and response options.
3. Eligible respondent universe.
4. Positive response code(s).
5. Treatment of Don't know and Refused.
6. Treatment of blank or not-applicable values.
7. Whether the measure is weighted.
8. Denominator used in the percentage.
9. Survey weight and any relevant design variables.
10. Whether the indicator is an ownership measure or an activity measure.

## Source documentation

Consult the [World Bank Global Findex](https://www.worldbank.org/en/publication/globalfindex) and the associated questionnaire, codebook and microdata documentation for the exact release used.
