# Dissertation

## Task Aims
- To understand whether fine tuning of BERT embeddings is required to detect hate speech to benchmark level on Facebook and Twitter.
- To understand the optimal model structure for the detection of Hate Speech on Facebook and Twitter, and to see if this is the same for Youtube and Reddit.
- To find out whether retraining of network weights is required to achieve benchmark performance on Youtube and Reddit. Here, we can deduce the similarities between the platforms and whether learnings from one can be applied to another.



## Task Methodology

- To optimise the detection of hate speech on a Twitter and Facebook dataset using three variations of DistilBERT transformer models.
- Experiment with two methods of transfer learning the ability to detect hate speech on a Youtube and Reddit dataset.

## Datasets
- Facebook and Twitter: HASOC 2019
- Youtube and Reddit: ETHOS

## Model Structures

1) DistilBERT for sequence classification (Frozen Embeddings and Network Weights)
2) DistilBERT for sequence classification (Dynamic Embeddings and Network Weights)
3) DistilBERT (Dynamic Embeddings and Network Weights) + Additional Bidirectional LSTM layer

## Transfer Learner Methods
1) Train architecture on Facebook and Twitter data, test directly on Youtube and Reddit.
2) Retrain architecture on Youtube and Reddit data.

## Conclusions

- Fine tuning of DistilBERT architecture on task specific data is required to achieve benchmark performance on Facebook and Twitter.
- An additional BLSTM layer with a dynamic DistilBERT architecture can achieve state of the art results on both datasets.
- Transfer learning method 2 is able to surpass state of the art results whereas transfer learning 1 is not able to, implying heterogeneity and the requirement to retrain network architectures.
