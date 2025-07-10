# Data Source Description

We will use data from the [General Social Survey](https://gss.norc.org/) (GSS), a biennial nationally representative survey of US adults that has been fielded since 1972. In 2008, the GSS first started asking about sexual orientation of respondents. We will pool the data from 2008-2018 to provide a larger sample of LGB individuals.

From the full data, I have extracted and recoded the following variables for our use as an analytical dataset. To load this dataset in R, you just need to run the setup code chunk in the full_report.Rmd R Markdown document. The name of the dataset in R is `gss`.

-   **noparents16**: This variable is coded as a "1" if the respondent indicated that they were not living with their parents at age 16 and that this had not been a result of parental death (i.e. not orphans). All other respondents received a "0". This is our key dependent variable. When we use this variable in models this term, the results will indicate the change in probability of not living with parents at age 16.
-   **sex_orient**: The sexual orientation of the respondent which is either "Heterosexual" or "Gay/Lesbian/Bisexual."
-   **age**: The age of the respondent.
-   **gender**: The gender of the respondent.
-   **reg16:** The region of the country that the respondent lived in at age 16.
-   **parent_educ**: The number of years of education of the parent of the respondent who had the highest education.
-   **raised_fund**: Whether the respondent was raised in a "Fundamentalist" or "Evangelical" faith. Either "Yes" or "No."
