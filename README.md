Data source: Thabtah, F. (2017). Autism Screening Adult [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5F019  

Includes: AQ-10 questionnaire scores, demographics, and family history.
704 observations, 20 predictors, 1 target variable (two classes).

Classification problem: Is Autism in adults indicated or not, based on AQ-10 Questions:

AQ-10 Questions:
A1_Score: I often notice small sounds when others do not.
A2_Score: I usually concentrate more on the whole picture, rather than the small details. (reverse scored)
A3_Score: I find it easy to do more than one thing at once. (reverse scored)
A4_Score: If there is an interruption, I can switch back to what I was doing very quickly. (reverse scored)
A5_Score: I find it easy to ‘read between the lines’ when someone is talking to me. (reverse scored)
A6_Score: I know how to tell if someone listening to me is getting bored. (reverse scored)
A7_Score: When I’m reading a story, I find it difficult to work out the characters’ intentions.
A8_Score: I like to collect information about categories of things (e.g., car types, bird species, train models).
A9_Score: I find it easy to work out what someone is thinking or feeling just by looking at their face. (reverse scored)
A10_Score: I find it difficult to work out people’s intentions.

The output of this questionnaire is intended to be used to suggest to support a pathway to formal diagnosis.
Machine learning models included Logistic Regression, Categorical Naive Bayes, and Support Vector Machines.
Thresholds for "does/not indicate Autism" were explored: Documentation set threshold score at >= 6; threshold in data was actually >= 7.
Sequential feature selection highlighted questionnaire results (AQ questions 5, 6, 9), region of residence, and ethnicity.

Naive Bayes ahad the best Confusion Matrix (max. true positives at 43, mini. false negatives at 9) and Test Accuracy (89.4%), while Logistic Regression had the best AUC (~93%).
