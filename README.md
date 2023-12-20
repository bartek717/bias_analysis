# bias_analysis

The objective of this project was to identify and mitigate biases present in language models. To accomplish this, I utilized the DistilBert model from the HuggingFace library, known for its efficiency in natural language processing. The project involved training the DistilBertForTokenClassification model to detect biased tokens, using a dataset with annotated biases.

A key aspect of the project was the development of a custom labeling function, process_data_to_labels, which prepared the dataset for training by assigning labels to tokens, indicating whether they were biased. This preparation was essential for effectively training the DistilBert model to recognize biased language.

Upon training, the model was equipped to identify biased tokens in texts processed by language models. To counteract the detected biases, I integrated the BertForMaskedLM model, which provided neutral alternatives to the biased words. This step was crucial in ensuring that the language models generated content that was not only accurate but also unbiased and fair.

I am looking to deploy the model live at some point to see how it detects bias, especially in open source models that havent been fine tuned.





