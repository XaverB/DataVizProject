# Stack Overflow Annual Developer Survey 2024

This dataset is derived from the 2024 Stack Overflow Annual Developer Survey. Conducted in May 2024, the survey gathered responses from over 65,000 developers across seven key sections:

1. Basic information
2. Education, work, and career
3. Tech and tech culture
4. Stack Overflow community
5. Artificial Intelligence (AI)
6. Professional Developer Series - Not part of the main survey
7. Thoughts on Survey

The dataset provided for this analysis focuses exclusively on the single-response questions from the main survey sections. Each categorical response in the survey has been integer-coded, with corresponding labels available in the crosswalk file.

What can you see about developer demographics? How do developers engage with Stack Overflow? What do they think about AI?

## Data Source

The data and description may be found on following GitHub repository:

[tidytuesday/data/2024/2024-09-03/readme.md at master · rfordatascience/tidytuesday · GitHub](https://github.com/rfordatascience/tidytuesday/blob/master/data/2024/2024-09-03/readme.md)

Three csv files contain all the data used in the study.

- https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2024/2024-09-03/qname_levels_single_response_crosswalk.csv
- https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2024/2024-09-03/stackoverflow_survey_questions.csv
- https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2024/2024-09-03/stackoverflow_survey_single_response.csv


## Data Dictionary

The data of the survey is divided into three csv files, containing the questions of the survey, the possible answers of each question and the survey results for each survey participant.

# `stackoverflow_survey_questions.csv`

Contains all questions asked in the survey, with an identification (qname) and the text represented in the survey.

|variable |class     |description |
|:--------|:---------|:-----------|
|qname    |character |Categorical Question/Column Name in main data |
|question |character |Text of the question as it was presented to the respondent |

# `qname_levels_single_response_crosswalk.csv`

Contains the possible answers of each question in the survey. The questions are referenced by the qname identification.

|variable |class     |description |
|:--------|:---------|:-----------|
|qname    |character |Categorical Question/Column Name in main data       |
|level    |integer   |Integer index associated with each column response       |
|label   |character |Label associated with integer index      |

# `stackoverflow_survey_single_response.csv`

Contains a list of all responses of the participants. One row contains all answers of each questions.

| variable              | class     | description                                                                         |
|:--------------------------|:-----------------|:--------------------------|
| response_id           | double    | Respondent ID                                                                       |
| main_branch           | integer   | Professional coding level of the respondent |
| age                   | integer   | Age                                                                                 |
| remote_work           | integer   | Current work situation                                                              |
| ed_level              | integer   | Highest education level completed                                                   |
| years_code            | integer   | Years the respondent has coded in total; More than 50 years coded as 51                 |
| years_code_pro        | integer   | Years the respondent has coded professionally; More than 50 years coded as 51                 |
| dev_type              | integer   | Best current-job description                                                        |
| org_size              | integer   | People in the organization                                                          |
| purchase_influence    | integer   | Level of influence in purchasing new technology at their organization                |
| buildvs_buy           | integer   | How much customization was needed in most recent tool recommendation |
| country               | character | Country in which the respondent lives |
| currency              | character | Currency of the country                                                             |
| comp_total            | double    | Total compensation                                                                  |
| so_visit_freq         | integer   | Stack Overflow visiting frequency                                                   |
| so_account            | integer   | Stack Overflow account status                                                       |
| so_part_freq          | integer   | Stack Overflow participation frequency                                              |
| so_comm               | integer   | Whether the respondent considers themself a member of the Stack Overflow community?                  |
| ai_select             | integer   | Use AI in development process                                                       |
| ai_sent               | integer   | Stance on using AI tools as part of development workflow                            |
| ai_acc                | integer   | Trust in accuracy of AI as part of development workflow                             |
| ai_complex            | integer   | How well the respondent believes the AI tools they use in development workflows handle complex tasks |
| ai_threat             | integer   | Belief that AI is a threat to current job |
| survey_length         | integer   | Feeling about the length of the Stack Overflow Developer Survey this year |
| survey_ease           | integer   | Ease of completion of this survey |
| converted_comp_yearly | double    | Converted compensation                                                              |
| r_used                | integer   | Flag if respondent used R in the previous year                                      |
| r_want_to_use         | integer   | Flag if respondent want to use R in the next year                                   |