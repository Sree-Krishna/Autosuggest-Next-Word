# Auto-Suggest Next Word

## Authors
- Sree Krishna Suresh
- Pareekshit Reddy Gaddam

## 1. Summary
Predicting the next word is a fundamental task in Natural Language Processing (NLP) with various applications, from minimizing keystrokes in typing to enhancing customer experience in search algorithms. This project explores different language model architectures, including n-gram models, Long Short-Term Memory (LSTM) neural networks, and Generative Pre-trained Transformer (GPT), to predict the next word in a sequence of text data. We evaluate these models using two text corpora: The Republic of Plato and The complete works of William Shakespeare.

## 2. Data
The dataset used in this project is obtained from Project Gutenberg, containing text files from various books and documents. We cleaned and tokenized the data, resulting in two datasets: Plato and Shakespeare. These datasets were preprocessed and split into training and testing sets for model evaluation.

## 3. Modeling
We implemented n-gram models with different sequence lengths, LSTM models using TensorFlow, and GPT-2 models using the Hugging Face library. Each model was trained and evaluated on the respective datasets, and perplexity was used as the evaluation metric.

## 4. Results
The table below summarizes the perplexity scores for each model on the Plato and Shakespeare datasets. Overall, the fine-tuned GPT-2 model outperformed other models, demonstrating the effectiveness of transformer-based models in language modeling tasks.

| Model           | Perplexity (Plato) | Perplexity (Shakespeare) |
|-----------------|---------------------|--------------------------|
| GPT-2 (Fine-tuned) | 7                 | 67                       |
| LSTM (Stacked)  | 194, 144, 136       | 239, 197, 164            |
| n-gram          | NA                  | 348, 481, 295            |

## 5. Future Works
Future enhancements to this project could include training models on larger corpora, improving model performance through multi-core GPU training, and extending models to predict multiple words or complete sentences. Additionally, exploring user-specific data for fine-tuning models could lead to practical applications such as email auto-completion.
