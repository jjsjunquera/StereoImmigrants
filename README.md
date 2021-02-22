# StereoImmigrants
StereoImmigrants is a  manually annotated dataset with stereotypes towards immigrants from ParlSpeech (https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/L4OAKN). 

The 'non-stereotypes.xlsx' file contains 2019 examples annotated as non-stereotypes towards immigrants, but still about the immigration topic.
The 'stereotypes.xlsx' file contains 1685 examples annotated with a specific stereotype category (i.e., Xenophobia's Victims;  Suffering Victims; Economical Resource;  Collective Threat; and Personal Threat).

Both files contain the following columns:
-COD_1: A random code to identify the speech.
-COD_2: A code to identify the sentence in its speech. The comcatenation of this code with the one of the speech gaves us a unique id for the labeled example.
-SENTENCE: The text that has been annotated.
-TAX_1: The label given by a social psichologist, regarding the categories and subcategories (i.e., frames) of the taxonomy proposed in [1]. 
Other colmuns contain the speach, speech's date, speaker and speaker's party.

The stereotypes examples have also manual annotation by 5 annotators who 
- labeled with the category or subcategory they concidered right in the case that they were not agree with TAX_1. (columns anno1, anno2, anno3, anno4, and anno5)
- labeled as pro-immigrant, anti-immigrant, or ambivalent, according to the feeling that the text produced after they read it.
The column T_TAX_1 has the category associated with the label in column TAX_1. For example, if the label from column TAX_1 is '1', the label in T_TAX_1 will be also '1'; but if the label in column TAX_1 is '1.1' specifying the first subcategory of Category '1', then the label in the column T_TAX_1 will keep only the firs digit i.e. '1'. 

In [1], we use the label of the column T_TAX_1 if at least three of the annotators agree that this is the right category.





[1]: the cite of the paper "Social Psychology based Taxonomy and StereoImmigrantsDataset for Identifying Stereotypes about Immigrants"



