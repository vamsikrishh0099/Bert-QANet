# Bert-QANet
Context Aware Question Answering Model Using QANet Architecture

This repository contains the code for a context-aware question answering model, which extends the QANet architecture to improve the understanding and response accuracy for questions requiring deeper context comprehension. The model effectively captures rich contextual information by incorporating both local and global interactions in the input text.

## Abstract

Traditional sequential question answering models often struggle to accurately understand and respond to questions that require a deeper understanding of context. To address this limitation, we propose a context-aware question answering model by extending the QANet architecture. Our model effectively models both local and global interactions in the input text, capturing rich contextual information.

In our experiments, we incorporated BERT embeddings into the input embedding layer, leveraging their success in capturing contextualized representations. We modified the model architecture to accommodate the larger dimensions of BERT embeddings. Additionally, we explored the impact of improving word embedding dimensions on the model’s trainable parameters, training time, and the number of attention heads required for comparable or better performance.

Comparing our approach with using glove word embeddings, we observed that the best performing BERT-QANet model achieved an F-1 score of 61.23, while the Glove-QANet model tended to saturate at a lower F-1 score of 58.27. Due to hardware constraints, we limited the training to 20 epochs, with each epoch taking approximately 2 hours.

Our findings suggest that utilizing context-aware word embeddings has the potential to enhance the performance of the QANet model in question answering tasks. However, it is important to note that this improvement comes at the cost of increased training time.

Getting Started:
Upload the jupyter notebook in Kaggle notebooks and we created our datasets and made it public on kaggle. Here are the links:
Add the datasets to your notebook. 
Connect to GPU on Kaggle and run all cells.
