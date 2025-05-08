# DeBERTa v3 Large News Classifier

This model is a fine-tuned version of [`microsoft/deberta-v3-large`](https://huggingface.co/microsoft/deberta-v3-large) for **multi-class classification of news headlines**.
The model classifies headlines into one of **7 categories**:

- World  
- Business  
- Technology  
- Entertainment  
- Sports  
- Science  
- Health

---

## Training Dataset

This model was trained on the [`logicalqubit/news_133k`](https://huggingface.co/datasets/logicalqubit/news_133k) dataset,  
which contains 133,000 labeled news headlines across the 7 categories mentioned above.

---

## Training Hyperparameters:

- learning_rate: 6e-6
- train_batch_size: 8
- eval_batch_size: 8
- warmup_steps: 50

- num_epochs: 2
- report_to: wandb

---

## Sample Code

![Demo Code](https://res.cloudinary.com/djk22geaj/image/upload/v1744489334/logicalqubitdeberta-v3-large-news-classifier_demo_code_k3sjqy.png)

---

## Sample Output

![Demo Output](https://res.cloudinary.com/djk22geaj/image/upload/v1744491408/logicalqubitdeberta-v3-large-news-classifier_demo_output_zzefym.png)

---

## Metrics

- While zero-shot models and fine-tuned text classification model differ fundamentally in design and purpose, this comparison is presented for reference. 
 It provides a practical benchmark, even if the comparison is entirely unfair.

![Metrics](https://res.cloudinary.com/djk22geaj/image/upload/v1744960519/f1scores_lmgxas.png)

![Metrics](https://res.cloudinary.com/djk22geaj/image/upload/v1744960519/inferenceTime_lbirwz.png)

---

## Wandb
 
![Wandb](https://res.cloudinary.com/djk22geaj/image/upload/v1744960554/wandb_train_q2cxgn.png)

![Wandb](https://res.cloudinary.com/djk22geaj/image/upload/v1744960555/wandb_eval_skue7a.png)

---
