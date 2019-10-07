# CONAN - COunter NArratives through Nichesourcing: a Multilingual Dataset of Responses to Fight Online Hate Speech

CONAN is a multilingual and expert-based dataset of hate speech/counter-narrative pairs for English, French and Italian.


## CONAN description
The dataset consists of 4,078 pairs over the 3 languages. Together with the data we also provide 3 types of metadata: expert demographics, hate speech sub-topic and counter-narrative type. The dataset is augmented through translation (from Italian/French to English) and paraphrasing, which brought the total number of pairs to 14.988. 

(\*)The original number was 15.024 but after post-hoc analysis, we deleted 9 original pairs (36 pairs including augmented ones) because they did not meet the required standard. 

## File description
In the [json file](https://github.com/marcoguerini/CONAN/blob/master/CONAN.json), each line starts with an ID, followed by a pair of hate speech/counter-narrative and the metadata (hate speech type, hate speech sub-topic, counter-narrative type, and demographics).

ID indicates language, hate speech type, hate speech sub-topic, unique hate speech count, counter-narrative count, and augmentation type (if any).

## ID example: 
FRT1ST0014HS0015CN001238T1

FR|T1|ST0014|HS0015|CN001238|T1

Language | HS Type | HS SubTopic | HS ID | CN Count | augmentation type (P1/P2/T1)

(P1: paraphrase 1 / P2: paraphrase 2 / T1: translation 1)

## Reference
You can find further details in the paper:

Y. Chung, E. Kuzmenko, S. S. Tekiroglu, M. Guerini, "CONAN - COunter NArratives through Nichesourcing: a Multilingual Dataset of Responses to Fight Online Hate Speech", Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics (ACL), 2019. Pdf available at: https://www.aclweb.org/anthology/P19-1271.pdf

## License
This resource can be used for research purposes. Please cite the publication above if you use it.
