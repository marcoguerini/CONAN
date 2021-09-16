# Hate countering (counter speech / counter narrative ) datasets
This repository contains hate countering datasets of:

- [CONAN](#CONAN)
- [Multitarget CONAN](#Multitarget-CONAN)
- [Knowledge-grounded hate countering dataset](#Knowledge-grounded-hate-countering-dataset)


# CONAN

CONAN is a multilingual and expert-based dataset of hate speech/counter-narrative pairs for English, French and Italian. 

## Dataset description
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

Yi-Ling Chung, Elizaveta Kuzmenko, Serra Sinem Tekiroğlu, and Marco Guerini. 2019. <em>CONAN - COunter NArratives through Nichesourcing: a Multilingual Dataset of Responses to Fight Online Hate Speech.</em> In Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics: Long Papers.

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
<!---
 # Multi-hate-target dataset using Human-in-the-Loop
-->

# Multitarget-CONAN

Multi-Target CONAN is a dataset of hate speech/counter-narrative pairs for English comprising several hate targets, collected using a Human-in-the-Loop approach. 

## Dataset description

The dataset consists of 5003 Hate Speech and Counter Narrative pairs covering the multiple hate targets, including DISABLED, JEWS, LGBT+, MIGRANTS, MUSLIMS, PEOPLE OF COLOR (POC), WOMEN. Each HS-CN pair is provided along with its loop information (VERSION), and its target (TARGET). 

The dataset is constructed using a novel human-in-the-loop data collection methodology in which a generative language model is refined iteratively by using its own data from the previous loops to generate new training samples that experts review and/or post-edit. Our experiments comprised several loops (versions) including dynamic variations. Multitarget_CONAN is the only expert-based multi-target HS/CN dataset available to the community.

## File description

Under the folder ```Multitarget-CONAN``` we provide the data in json, xlsx, and csv format. Each entry has a unique index and has four fields: HATE_SPEECH, COUNTER_NARRATIVE, VERSION, and TARGET. 

## Citation
You can find further details in our paper:

Margherita Fanton, Helena Bonaldi, Serra Sinem Tekiroğlu, Marco Guerini <em>Human-in-the-Loop for Data Collection: a Multi-Target Counter Narrative Dataset to Fight Online Hate Speech</em> In Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics: Long Papers.

```bibtex
@inproceedings{fanton-2021-human,
  title="{Human-in-the-Loop for Data Collection: a Multi-Target Counter Narrative Dataset to Fight Online Hate Speech}",
  author="{Fanton, Margherita and Bonaldi, Helena and Tekiroğlu, Serra Sinem and Guerini, Marco}",
  booktitle = "Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics",
  month = aug,
  year = "2021",
  publisher = "Association for Computational Linguistics",
}
```

# Knowledge-grounded hate countering dataset

This small dataset contains hate speech/counter-narrative pairs coupled with the backgroud knowledge used to construct the counter-narrative. 

## Dataset description

The dataset consists of 195 HS-CN pairs covering multiple hate targets (islamophobia, misogyny, antisemitism, racism, and homophobia), provided along with the relevant knowledge automatically retrieved.

The counter narratives are written by an expert who is tasked with composing a suitable CN response to a given hate speech using the corresponding knowledge as much as possible.

## File description
Under the folder ```multitarget_KN_grounded_CN``` we provide the data in json and csv format. In the files, each entry has four fields: hate speech, knowledge sentences, counter narrative, and target. 

## Citation
You can find further details in our paper:

Yi-Ling Chung, Serra Sinem Tekiroğlu, and Marco Guerini. 2021. <em>Towards Knowledge-Grounded Counter Narrative Generation for Hate Speech.</em> In Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics: Findings.


```bibtex
@inproceedings{chung-etal-2021-knowledge,
    title = "{Towards Knowledge-Grounded Counter Narrative Generation for Hate Speech",
    author = "Chung, Yi-Ling and Tekiroğlu, Serra Sinem and Guerini, Marco",
    booktitle = "Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics",
    month = aug,
    year = "2021",
    address = "Online",
    publisher = "Association for Computational Linguistics",
}
```


## License
These resources can be used for research purposes. Please cite the corresponding publication if you use it.
