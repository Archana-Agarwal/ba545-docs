<<<<<<< HEAD
# BA 545 Course Project 1: Advanced Preparation of Financial Data
## Spring 2020

## Overview of the Competition

Understanding pricing strategies in the context of the Initial Public Offering (IPO) process has been receiving much attention. Most prior studies have however focused on information sources from post issuance periods, and understanding such strategies from the management’s perspective during the IPO process is still an open research issue. Form 424 variants, as finalized IPO prospectus approved by Security Exchange Committee (SEC), contain rich and genuine information about the issuing firms. In this study, we analyze the inter-relationships between the management’s confidence (through the proxy of sentiments expressed in textual contents in the Management’s Discussion & Analysis (MD&A) sections in the prospectus) and the pre-/post-IPO valuations.

In this competition, you are provided with data regarding successful U.S. IPOs from __more than 600 companies__. Your client is seeking advanced and novel methods to __prepare the collected data__, for further predictive analysis of the “underpricing” phenomenon. You will mainly focus on the data understanding and data preparation phases in the CRISP-DM model. Advanced preparation and modeling techniques will be needed for extra points.

## General Information about the Competition
- Started: __12:00 AM ETC, Jan. 28th, 2020, Tuesday__
- Milestone Checkpoint: __11:59 PM ETC, Feb. 11th, 2020, Tuesday,__
- Submission Deadline: __11:59 PM ETC, Feb. 25th, 2020, Tuesday__
- Points: __200__ points in total, 100 points in each part – see __Evaluation Rules__ for details.

## Competition Rules
Please find the generic competition rules below. Dr. Tao reserves all the rights to further explain the rules.

### Participation Rules
- All participants __have to be__ in groups; every group contains __3__ students.
- Privately sharing data, codes, or any other artefacts outside of the groups is __not permitted__ – once violated, the group
will be __disqualified__ from the competition.
- Group leaders have full authority over the group – the communications between groups, or between groups and Dr.
Tao should __only__ be conducted by group leaders.

### Submission Rules
- Only __one (1)__ final submission can be made by each group.
- __Unlimited__ submissions can be made before the checkpoint deadline – which will not be graded.
- __No late submissions__ (after submission deadline) will be accepted.
- Each submission contains (fail to submit any part may lead to the disqualification of the competition):
  - The __data file__ prepared by the group;
  - The __python workflow__ (in Jupyter Notebooks) and/or any other code used by the group; 
  - __Detailed comments and explanations__ to all the code used.
 
### Evaluation Rules
- Submissions are evaluated on __two evaluation metrics__ of the modeling results; each part takes up to __100__ points:
  - _Prediction Accuracy_: we will use F-1 score as the measurement of how close the predicted values are to the factual outputs – please refer to [this Wikipedia article](https://en.wikipedia.org/wiki/Precision_and_recall) for the computation of F-1 score;
  - _Predictive Power_: we will use __ROC curve__ (Receiver Operating Characteristics), or similarly, AUC (Area Under ROC Curve), is a graphical representation that demonstrate the predictive performances of models. Note that ROC/AUC can only be applied to __binary targets__. The rule-of-thumb for ROC is as follows (the higher the better):
  
 | AUC Value | Interpretation |
:--- | :---
| 1.0 | Perfect Analysis |
| 0.9 - 0.99 | Excellent Analysis |
| 0.8 - 0.89 | Good Analysis |
| 0.7 - 0.79 | Fair Analysis |
| 0.5 - 0.69 | Poor Analysis |
| 0.5 and Below | Worthless Analysis |

- Submissions are ranked base on F1-score and AUC, respectively. All groups' performances are ranked - the groups ranked top 3 in class are rewarded with extra points: 

  + First place: 20 extra points
  + Second place: 10 extra points
  + Third place: 5 extra points

- Every submission will be evaluated by Dr. Tao and at least one (1) independent judge – all disagreements need to be resolved before release the results to the participants. __Example evaluation code will be provided for your convenience.__

- Extra point opportunities: each group can make use of up to one (1) extra points opportunity – each opportunity worth up to 10 extra points:
  + __More modeling techniques__: the basic modeling technique being used for evaluation is (logistic) regression model(s) – if you can find more applicable modeling techniques (decision tree, neural network, etc.) and apply them as your evaluation technique(s), you will receive __up to 10 extra points__;
  + __More preprocessing techniques__: If you can use any data preprocessing step __other than__ the suggested tasks on the next page – you will receive __up to 10 extra points__;
  + You need to notify Dr. Tao your group’s decision regarding the extra point opportunities no later than 11:59 PM, Tuesday, February 11th, 2020 ETC.
  
## Competition Guidelines

### Research Question
The overarching research question is “ _What are the determinants of IPO underpricing phenomena?_ ” In this competition, your main purpose is to prepare the data for predictive models answering the overarching research question.

### Data Dictionary
See attached ‘Data Dictionary’ Document.

### Suggested Tasks
Following tasks are normally conduct in data preparation phase. __Not all steps are required/available in this particular dataset__ – and __not in this particular order__. Some additional step(s) might be required – which you might need to research on. Keep in mind that your decisions on different strategies below will determine the results.

1. __Descriptive statistics__ – describing the data using minimum, maximum, 1st & 3rd quartile, mean, median, standard deviation, number of records, number of missing records, ...
2. __Imputation__ – dealing with missing data, you can choose from following strategies: 
  i) drop the record with missing (highly discouraged); 
  ii) replace the missing with mean/median/mode, determined on the data type; 
  iii) replacing missing values in continuous field with linear regression predictions;
3. __Normalization__ – You need to manipulate all continuous fields to follow normal distribution: which contains two steps: 
  i) removing skewness (using logarithm, square root, etc.) 
  ii) make sure the residual is randomly distributed;
4. __Correlation analysis__ – you need to select predictor variables with low pair-wise correlation (i.e. spearman’s) values – usually the threshold is __0.5__ – one variable from the pair should be excluded from the model;
5. __Standardization__ – you need to convert the values at the same numeric level; one way of doing this is to use the z-score standardization, which is calculated as shown on [this page](https://www.statisticshowto.datasciencecentral.com/probability-and-statistics/z-score/).
6. __Recoding__ – for categorical data, you might want to recode them. For instance, since you need to use AUC as the evaluation metric, you should convert the target(s) to binary (two classes). Also, you should recode any categorical variable(s) with no more than 5 classes.

### Additional Rules
- If you decide to include/exclude certain variable(s)/observation(s) from the dataset, you will need to __get approved from Dr. Tao__;
- You will need to report your __workload allocation__ (within the group) in the Milestone report and the final report – non-equal workload assignment will lead to the penalty to the whole group;
- If cross-group collaboration is identified, __both groups will be disqualified from the competition__ (result in 0 points for this part of the course).
=======
# BA 545 Course Documents
_Spring 2020_

## Table of Contents
+ [Syllabus](https://github.com/DrJieTao/ba545-docs/blob/master/syllabus.md)
+ [Agendas](https://github.com/DrJieTao/ba545-docs/tree/master/Agendas)
+ Lecture Slides (on Google Docs, can be found in each week's agenda)
+ In Class Tutorials (Jupyter Notebooks, can be found using each week's link to Github Classroom)
+ [Competition#1](https://github.com/DrJieTao/ba545-docs/tree/master/competition1)
+ [Competition#2](https://github.com/DrJieTao/ba545-docs/tree/master/competition2)
+ Downloads (To Be Updated)
+ [JuoyterHub User Guide](https://github.com/DrJieTao/ba545-docs/blob/master/1_28_2019%20JupyterHub-Guide.pdf)
  + Special thanks to Ms. Pu for preparing this document. If you have any technical issues, please contact [Ms. Pu](mailto:yue.pu@student.fairfield.edu).

>>>>>>> 3b9f8be75e340b002afcc4724b810fc9e158554d
