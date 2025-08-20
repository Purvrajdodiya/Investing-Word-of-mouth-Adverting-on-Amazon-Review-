# Investigating Word of Mouth Advertising

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning/Preparation](#data-cleaningpreparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results/Findings](#resultsfindings)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)

### Project Overview
---

This project investigates the impact of humor and grammatical errors in online product reviews on consumer behavior. The study aims to understand how these two factors influence a potential customer's perception of a review's value and their intention to purchase a product. By analyzing reactions to different styles of reviews for products like books and home appliances, the research seeks to determine whether humor can increase a review's effectiveness and to what extent poor grammar detracts from its credibility. The findings will provide insights into the key elements that make electronic word-of-mouth (eWOM) a powerful tool in the digital marketplace.


### Data Sources
---
The primary data was collected from 102 individuals through an online questionnaire. After removing incomplete responses, the final dataset consisted of responses from 67 participants. The data includes demographic information (age, gender) and ratings on product reviews based on humor, grammar, perceived value, and purchase intention. The product reviews used as stimuli were adapted from actual reviews on Amazon for a book ("The Alchemist" by Paulo Coelho) and a vacuum cleaner (Dyson Ball Animal 2).

### Tools
---
- **Excel** - Data Cleaning
- **Qualtrics** - Survey design and data collection.
- **Jamovi (Version 2.3)** - Statistical analysis (T-tests, ANOVA).
- **R (Version 4.1)** - Underlying statistical computing for Jamovi.

### Data Cleaning/Preparation
---
In the initial data preparation phase, the following tasks were performed:
1.  **Data Inspection:** The initial dataset of 102 participants was reviewed for completeness.
2.  **Handling Missing Values:** 35 participants were removed from the dataset due to incomplete responses, resulting in a final sample size of 67.
3.  **Assumption Checking:** The data was checked for normality. A non-parametric Kruskal-Wallis test was conducted due to the small sample size and non-normal distribution.

### Exploratory Data Analysis
---
EDA involved exploring the data to answer key questions, such as:

-   How valuable are humorous reviews perceived to be compared to non-humorous ones?
-   Do spelling and grammatical errors negatively impact the perceived value of a review?
-   Are participants more likely to purchase a product after reading a funny review?
-   Does the impact of humor and grammar differ between product types (e.g., a book vs. a vacuum cleaner)?

### Data Analysis
---
A series of 2x2 factorial ANOVAs were conducted to examine the influence of humor (funny vs. not funny) and spelling/grammar (error vs. no error) on the perceived value of the review and the likelihood of purchasing the product.

```
ANOVA - valuable book

| | Sum of Squares | df | Mean Square | F | p |
| :--- | :--- | :--- | :--- | :--- | :--- |
| funny BOOK | 16.873 | 1 | 16.873 | 6.531 | 0.013 |
| spelling grammar book | 20.988 | 1 | 20.988 | 8.123 | 0.006 |
| funny BOOK * spelling grammar book | 0.291 | 1 | 0.291 | 0.113 | 0.738 |
| Residuals | 157.601 | 61 | 2.584 | | |
```

### Results/Findings
---
The analysis results are summarized as follows:
1.  **Humor increases purchase intention and perceived value.** Funny reviews consistently received higher ratings for both the book and the vacuum cleaner, suggesting humor is a key factor in shaping positive consumer attitudes.
2.  **Grammatical errors reduce perceived value.** Reviews without spelling or grammar errors were perceived as more valuable, particularly for the book, which is a text-based product.
3.  **Humor can sometimes override poor grammar.** In one notable exception, a funny review with spelling errors for the book resulted in higher purchase intentions than a non-funny, error-free review.

### Recommendations
---
Based on the analysis, we recommend the following actions for businesses and marketers:
-   Strategically incorporate humor into online review platforms and marketing content to increase consumer engagement and boost purchase intentions.
-   Encourage reviewers or brand ambassadors to use engaging but error-free language to convey both credibility and appeal.
-   Marketing teams should provide guidelines that emphasize clear and correct language to maintain a high standard of quality in user-generated content.

### Limitations
---
The primary limitation of this study is the small sample size (N=67), which may not be generalizable to the broader population. The participant demographic was also relatively young (mean age of 27), which could skew the results. Furthermore, the study only included two product types; a wider variety of products might yield different results.

### References
---
1.  Eisend, M. (2009). A meta-analysis of humor in advertising. *Journal of the Academy of Marketing Science*, 37(2), 191–203.
2.  Cooper, A. E., Diab, D. L., & Beeson, K. M. (2020). Why Spelling Errors Matter: Online Company Reviews and Organizational Attraction. *Corporate Reputation Review*, 23(3), 160–169.
3.  The jamovi project (2022). jamovi. (Version 2.3) [Computer Software]. Retrieved from https://www.jamovi.org.
