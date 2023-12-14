# UN COFOG Classifier-
This classifier was developed utilizing the pre-trained BERT (Bidirectional Encoder Representations from Transformers) model with an uncased configuration, with over 1500 manually labeled dataset comprising budget line items extracted from various budgetary documents. To balance the data, additional data was generated using GPT-4 where categories were not available in budget documents. The model training was executed on a Google Colab environment, specifically utilizing a Tesla T4 GPU. The model is designed to predict the primary classification level of the Classification of the Functions of Government (COFOG), with the predictions from the first level serving as contextual input for subsequent second-level classification. The project is conducted with an exclusive focus on academic and research objectives. Detailed metrics of the training process are as follows:

You Can test and download model from (HuggingFace)[https://huggingface.co/spaces/peterkros/COFOG-Bert-AutoClassifier]

```TrainOutput(global_step=395, training_loss=1.1497593360611156, 
    metrics={'train_runtime': 650.0119, 'train_samples_per_second':
      9.638, 'train_steps_per_second': 0.608, 'total_flos': 1648509163714560.0, 
      'train_loss': 1.1497593360611156, 'epoch': 5.0})
```

-------------
