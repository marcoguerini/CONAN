# Hate countering datasets
This repository contains hate countering datasets of:

- [CONAN](#CONAN)
- [Multi-hate-target knowledge-grounded hate countering dataset](#Multi-hate-target-knowledge-grounded-hate-countering-dataset)


# CONAN

## COunter NArratives through Nichesourcing: a Multilingual Dataset of Responses to Fight Online Hate Speech

CONAN is a multilingual and expert-based dataset of hate speech/counter-narrative pairs for English, French and Italian.

## CONAN description
The dataset consists of 4,078 pairs over the 3 languages. Together with the data we also provide 3 types of metadata: expert demographics, hate speech sub-topic and counter-narrative type. The dataset is augmented through translation (from Italian/French to English) and paraphrasing, which brought the total number of pairs to 14.988. 

(\*)The original number was 15.024 but after post-hoc analysis, we deleted 9 original pairs (36 pairs including augmented ones) because they did not meet the required standard. 

## File description
Under the folder ```CONAN``` we provide the dataset in json and csv format. In the files each entry starts with an ID, followed by a pair of hate speech/counter-narrative and the metadata (hate speech type, hate speech sub-topic, counter-narrative type, and demographics).

ID indicates language, hate speech type, hate speech sub-topic, unique hate speech count, counter-narrative count, and augmentation type (if any).

## ID example: 
FRT1ST0014HS0015CN001238T1

FR|T1|ST0014|HS0015|CN001238|T1

Language | HS Type | HS SubTopic | HS ID | CN Count | augmentation type (P1/P2/T1)

(P1: paraphrase 1 / P2: paraphrase 2 / T1: translation 1)

## Citation
You can find further details in our paper:

```bibtex
@inproceedings{chung-etal-2019-conan,
    title = "{CONAN} - {CO}unter {NA}rratives through Nichesourcing: a Multilingual Dataset of Responses to Fight Online Hate Speech",
    author = "Chung, Yi-Ling and Kuzmenko, Elizaveta and Tekiroglu, Serra Sinem and Guerini, Marco",
    booktitle = "Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics",
    month = jul,
    year = "2019",
    address = "Florence, Italy",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/P19-1271",
    doi = "10.18653/v1/P19-1271",
    pages = "2819--2829"
}
```

# Multi-hate-target knowledge-grounded hate countering dataset

## Dataset description

The dataset consists of 195 HS-CN pairs covering multiple hate targets (islamophobia, misogyny, antisemitism, racism, and homophobia), provided along with the relevant knowledge automatically retrieved.

The counter narratives are written by an expert who is tasked with composing a suitable CN response to a given hate speech using the corresponding knowledge as much as possible.

## File description
Under the folder ```multitarget_KN_grounded_CN``` we provide the data in json and csv format. In the files, each entry has four fields: hate speech, knowledge sentences, counter narrative, and target. 

## Citation
You can find further details in our paper:

Yi-Ling Chung, Serra Sinem Tekiroglu, and Marco Guerini. 2021. <em>Towards Knowledge-Grounded Counter Narrative Generation for Hate Speech.</em> In Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics: Findings.

<!---
```bibtex
@inproceedings{chung-etal-2021-knowledge,
    title = "{Towards Knowledge-Grounded Counter Narrative Generation for Hate Speech",
    author = "Chung, Yi-Ling and Tekiroglu, Serra Sinem and Guerini, Marco",
    booktitle = "Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics",
    month = aug,
    year = "2021",
    address = "Online",
    publisher = "Association for Computational Linguistics",
}
```
-->

## License
This resource can be used for research purposes. Please cite the publication above if you use it.
