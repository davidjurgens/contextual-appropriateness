#  	Your spouse needs professional help: Determining the Contextual Appropriateness of Messages through Modeling Social Relationships

This repository contains the code for the ACL 2023 paper "Your spouse needs professional help: Determining the Contextual Appropriateness of Messages through Modeling Social Relationships". 

**Abstract:** 
> Understanding interpersonal communication requires, in part, understanding the social context and norms in which a message is said. However, current methods for identifying offensive content in such communication largely operate  independent of context, with only a few approaches considering community norms or prior conversation as context. Here, we introduce a new approach to identifying inappropriate communication by explicitly modeling the social relationship between the individuals. We introduce a new dataset of contextually-situated judgments of appropriateness and show that large language models can readily incorporate relationship information to accurately identify appropriateness in a given context.  Using data from online conversations and movie dialogues, we provide insight into how the relationships themselves function as implicit norms and quantify the degree to which context-sensitivity is needed in different conversation settings. Further, we also demonstrate that contextual-appropriateness judgments are predictive of other social factors expressed in language such as condescension and politeness.

# Summary

The repository is roughly broken up as follows

* `data/`: the dataset in its train, dev, and test splits, and a dataframe with the high-level categories of each relationship
* `src/data`: Contains basic preprocessing for Phase 2 of the data annotation
* `src/model`: Code for training and testing the contextual appropriateness model and the downstream models for Politeness and Condescension
* `src/visualization`: Code for the plots in the downstream analyses

# Citation

```
@inproceedings{jurgens2023your,
    title = "Your spouse needs professional help: Determining the Contextual Appropriateness of Messages through Modeling Social Relationships",
    author = "Jurgens, David and Seth, Agrima and Sargent, Jackson and Aghighi, Athena and Geraci, Michael ",
    booktitle = "Proceedings of the 60th Annual Meeting of the Association for Computational Linguistics",
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    pages = "504--522",
}
```

