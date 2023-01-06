# MADS-milestone-2-SIADS-696
Milestone 2 project

Team members:
  - Manish Jakhi
  - Koustubh Jadhav


Introduction:
Health care professionals manually convert diagnosis reports into ICD codes for billing and insurance purposes. There are 160K ICD codes and a large number of patient data that gets processed in each hospital.
ICD codes, as they are standardized, are the one of the consistent ways to indicate the diagnosis and procedure that were carried out for a particular patient during his/her admission.
Diagnosis codes are extracted from medical records for billing, insurance and reimbursement purposes. This is a manual process and is usually done by experienced individuals by referring to the documented medical records. These codes systematically represent the diagnosis conditions the patient was treated in the hospital facility.
ICD-9 codes contain 3 to 5 digits and are organized hierarchically. They are usually represented as abc.xy where the first three characters are the main disease category, while the x and y components represent subdivisions of the abc category.
ICD 9 code example 

![image](https://user-images.githubusercontent.com/55030743/211115451-9d87fdc0-30f7-44af-9a39-f17d1830f738.png)

There are more than 1300 ICD categories. For the scope of this project we are only focusing On determining the correct ICD category. ICD coding scheme and standard is used by many healthcare organizations and hospitals.
Assigning of the diagnosis codes is a very tedious process and although it is done by trained professionals it is prone to errors and inconsistencies. The coder has to go through hundreds if not thousands lines of text to extract the right information so that correct ICD codes can be billed for a particular individual.

In this report using a combination of unsupervised and supervised machine learning we have tried to extract international classification of diseases, clinical modification, 9th revision (ICD-9-CM) diagnosis codes from electronic health records (EHRs).

Our goal with this is not to come up with an automated process of assigning ICDs which will replace trained coders, but to expedite coding and provide consistent coding outcome by providing a list of relevant ICDs from discharge summary for the coders to choose from.

Assigning of the ICD diagnosis codes is a very tedious process and although it is done by trained professionals it is prone to errors and inconsistencies. The coder has to go through hundreds if not thousands lines of text to extract the right information so that correct ICD codes can be billed for a particular individual. 
In this report using a combination of unsupervised and supervised machine learning we will try to extract international classification of diseases, clinical modification, 9th revision (ICD-9-CM) diagnosis codes from electronic health records (EHRs).

Our goal with this is not to come up with an automated process of assigning ICDs which will replace trained coders, but to expedite coding and provide consistent coding outcome by providing a list of relevant ICDs from discharge summary for the coders to choose from.

We used the LDA unsupervised learning method for topic modeling of patient discharge summary, and used it for data exploration and to extract document topic vectors as features. Our goal was to predict ICD code assignment associated with the patient discharge summary and for that we used the multi label classification supervised learning approach. We were able to achieve higher evaluation metric scores using topic vectors as features. We constructed models which can predict 50, 100 and 250 most commonly used ICDs. We observed that considering fewer ICDs for prediction results in higher model evaluation metric scores.


