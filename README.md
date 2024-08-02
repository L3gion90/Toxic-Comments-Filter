Toxic Comments Filter

We will build a model capable of filtering user comments according to the degree of harmfulness of the language:

1. Preprocess the text by eliminating tokens that do not make a significant contribution at the semantic level.
2. Transform the text corpus into sequences.
3. Build a deep learning model with recurrent layers for a multi-label classification task.
4. At prediction time, the model must return a vector containing a 1 or a 0 for each label in the dataset (toxic, severe_toxic, obscene, threat, insult, identity_hate).
   In this way, a non-hazardous comment will be classified by a vector containing only 0s [0,0,0]. Conversely, a dangerous comment will have at least a 1 among the 6 labels.
