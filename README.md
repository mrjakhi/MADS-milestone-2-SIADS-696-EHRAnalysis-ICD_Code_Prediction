# MADS-milestone-2-SIADS-696
Milestone 2 project

Team members:
  - Manish Jakhi
  - Koustubh Jadhav

Assigning of the ICD diagnosis codes is a very tedious process and although it is done by trained professionals it is prone to errors and inconsistencies. The coder has to go through hundreds if not thousands lines of text to extract the right information so that correct ICD codes can be billed for a particular individual. 
In this report using a combination of unsupervised and supervised machine learning we will try to extract international classification of diseases, clinical modification, 9th revision (ICD-9-CM) diagnosis codes from electronic health records (EHRs).

Our goal with this is not to come up with an automated process of assigning ICDs which will replace trained coders, but to expedite coding and provide consistent coding outcome by providing a list of relevant ICDs from discharge summary for the coders to choose from.

We used the LDA unsupervised learning method for topic modeling of patient discharge summary, and used it for data exploration and to extract document topic vectors as features. Our goal was to predict ICD code assignment associated with the patient discharge summary and for that we used the multi label classification supervised learning approach. We were able to achieve higher evaluation metric scores using topic vectors as features. We constructed models which can predict 50, 100 and 250 most commonly used ICDs. We observed that considering fewer ICDs for prediction results in higher model evaluation metric scores.
