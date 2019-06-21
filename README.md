# CONAN - COunter NArratives through Nichesourcing: a Multilingual Dataset of Responses to Fight Online Hate Speech

CONAN is a multilingual and expert-based dataset of hate speech/counter-narrative pairs for English, French and Italian.


## CONAN description
The dataset consists of 4078 pairs over the 3 languages. Together with the data we also provid 3 types of metadata: expert demographics, hate speech sub-topic and counter-narrative type. The dataset is augmented the dataset through translation (from Italian/French to English) and paraphrasing which brought the total number of pairs to more than 15 thousand. 


## File description
In the json file, each line starts with an ID, followed by a pair of hate speech/counter-narrative and the metada (demographics of the counter-narrative).

ID indicates languages, hate speech type, hate speech subtype, unique hate speech count, counter-narrative count, and augmentation type (if any).

# ID example: 
FR|T1|ST0014|HS0015|CN001238|T1 #FRT1ST0014HS0015CN001238T1

Language + HS Type + HS Subtype + unique HS ID + CN Count + augmentation type (P1/P2/T1)

P1 : paraphrase 1 
P2 : paraphrase 2
T1 : translation 1


# References
For further details please find reference in the following BibTex entry:

Y. Chung, E. Kuzmenko, S. S. Tekiroglu, M. Guerini, "CONAN - COunter NArratives through Nichesourcing: a Multilingual Dataset of Responses to Fight Online Hate Speech", Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics (ACL), 2019.

## License
