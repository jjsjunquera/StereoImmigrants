# StereoImmigrants
StereoImmigrants is a  manually annotated dataset with stereotypes towards immigrants from Spanish speeches in the ParlSpeech dataset (https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/L4OAKN). 

The 'non-stereotypes.xlsx' file contains 2019 examples annotated as non-stereotypes towards immigrants, but still about the immigration topic.
The 'stereotypes.xlsx' file contains 1685 examples annotated with a specific stereotype category (i.e., Xenophobia's Victims;  Suffering Victims; Economical Resource;  Collective Threat; and Personal Threat).

Both files contain the following columns:
- COD_1: A random code to identify the speech.
- COD_2: A code to identify the sentence in its speech. The comcatenation of this code with the one of the speech gaves us a unique id for the labeled example.
- SENTENCE: The text that has been annotated.
- TAX_1: The label given by a social psichologist, regarding the categories and subcategories (i.e., frames) of the taxonomy proposed in [1]. 
Other colmuns contain the speach, speech's date, speaker and speaker's party.

The stereotypes examples have also manual annotation by 5 annotators who 
- labeled with the category or subcategory they concidered right in the case that they were not agree with TAX_1. (columns anno1, anno2, anno3, anno4, and anno5)
- labeled as pro-immigrant, anti-immigrant, or ambivalent, according to the feeling that the text produced after they read it. (columns eva1,	eva2,	eva3,	eva4,	eva5)
The column T_TAX_1 has the category associated with the label in column TAX_1. For example, if the label from column TAX_1 is '1', the label in T_TAX_1 will be also '1'; but if the label in column TAX_1 is '1.1' specifying the first subcategory of Category '1', then the label in the column T_TAX_1 will keep only the firs digit i.e. '1'. 

For the experiment we did in [1], we use the texts and their label of the column T_TAX_1, if at least three of the annotators agree that this is the right category.
Because of the texts' lenght and the prejudice expert valoration, we exclude the texts with the following codes (concatenation of COD_1-COD_2):
"5201-9", "1105-28", "1682-4", "4743-7", "4752-4", "1105-32", "4711-34", "4743-23", "1105-33", "4743-20",
"1859-14", "4713-48", "4743-21", "911-1", "4457-6", "834-19", "1105-14", "1105-24", "4711-33", "707-9",
"4711-36", "4711-79", "4711-88", "1105-29", "4317-3", "778-1", "881-5", "2075-1", "2558-35", "4365-1",
"4393-23", "4987-8", "899-1", "1003-18", "1337-21", "4393-11", "4393-40", "4453-56", "4457-1", "1105-11",
"834-1", "552-1", "1118-1", "829-3", "846-3", "1434-15", "1859-1"





[1]: the cite of the paper "Social Psychology based Taxonomy and StereoImmigrantsDataset for Identifying Stereotypes about Immigrants"



