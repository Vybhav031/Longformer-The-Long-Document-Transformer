# Longformer-The-Long-Document-Transformer
### Project overview :
The Longformer model is introduced as a solution to the limitations of standard Transformer architectures, which struggle with long sequences due to the quadratic scaling of the self-attention mechanism. The Longformer employs a novel attention mechanism that combines a local windowed attention pattern with task-motivated global attention. This approach allows the model to efficiently process documents with thousands of tokens, maintaining contextual integrity over long sequences. The Longformer was evaluated on language modeling tasks and various downstream NLP tasks, including question answering and document classification, consistently outperforming baseline models like RoBERTa on tasks involving long sequences. By addressing the computational inefficiencies of traditional Transformers, the Longformer opens up new possibilities for effectively handling long-range dependencies in natural language processing tasks.
### AIM :
The primary objective of this project is to implement the Longformer model, which introduces an efficient attention mechanism that scales linearly with sequence length, thereby enabling the processing of long documents without the quadratic complexity inherent in traditional Transformer models. This project evaluates the Longformer in various NLP tasks to demonstrate its capability to handle long sequences. By leveraging the unique architecture of the Longformer, the project aims to explore its effectiveness in improving performance on tasks that require understanding and processing of long documents, thereby offering insights into its potential applications and optimizations in real-world scenarios.
### Dataset :
The Longformer was evaluated using a variety of datasets that necessitate the handling of long contexts. These include WikiHop, TriviaQA, and HotpotQA, among others. These datasets are specifically selected to showcase the model's effectiveness in scenarios where capturing long-range dependencies is crucial. Each dataset provides a different challenge, allowing the Longformer to demonstrate its ability to maintain context and understanding across extensive text sequences. 
Here i could not upload the dataset as it was larger but you can download it from the codes i have provided in notebook.
### Description :
The implementation of the Longformer model for this project was primarily based on the publicly available Longformer GitHub Repository, which provides the foundational code for the model. This repository serves as a starting point for setting up and running the Longformer on various NLP tasks. The initial phase of the implementation involved configuring the Longformer model to operate on selected datasets, including those that require processing long sequences to capture extended context effectively.
* The implementation process included downloading the datasets, preprocessing the data to match the input requirements of the Longformer, and integrating the model with the existing infrastructure for training and evaluation. This setup ensured that the model could leverage its novel attention mechanism efficiently to handle tasks such as document classification, question answering, and summarization. Additionally, the code was organized to facilitate easy experimentation with different configurations and parameter settings, enabling thorough evaluation across multiple tasks.
* Modifications
To tailor the Longformer implementation to the specific needs of the project, several modifications and enhancements were introduced:
**Dataset-Specific Adjustments**:
The original code was modified to accommodate the unique requirements of the selected datasets. This involved adjusting data loading and preprocessing routines to ensure compatibility with the Longformer's input format. Special care was taken to preserve the sequence length and context, which are crucial for the model's performance on long document tasks.
**Custom Evaluation Metrics**:
The base implementation was extended to include custom evaluation metrics that were not initially part of the repository. These metrics provided more detailed insights into model performance by focusing on key aspects such as evaluation loss, runtime efficiency, and the impact of hyperparameter variations. This allowed for a more comprehensive assessment of how different settings affected the model's outcomes.
**Hyperparameter Optimization**:
The code was adapted to optimize critical hyperparameters, including learning rates and batch sizes, which are vital for enhancing model performance. A series of experiments were conducted to identify the optimal configurations for these parameters, enabling the Longformer to achieve improved results on the chosen tasks. The implementation was structured to allow for easy adjustment of these parameters, facilitating rapid testing and fine-tuning.
**Integration with Training and Evaluation Frameworks**:
The Longformer model was integrated with established training and evaluation frameworks to streamline the experimentation process. This included setting up the Trainer class from the transformers library, which provided a robust infrastructure for conducting experiments and collecting results. This integration ensured efficient training cycles and facilitated the systematic exploration of different model configurations.
### Installation :
To run this project, follow the steps below:
Clone the repository and then 
you can use this following command in your terminal or command prompt 'git clone

### Usage :
To run the project, open the Final_Project.ipynb notebook in a Jupyter environment. Download the dataset the dataset. Then, run the cells sequentially. This will load the dataset, perform data preprocessing, train various machine learning models, and evaluate their performance.
### Paperswithcode :
https://paperswithcode.com/paper/longformer-the-long-document-transformer
### Githubcloned :
https://github.com/allenai/longformer
### Reference : 
 Beltagy, I., Peters, M. E., & Cohan, A. (2020). Longformer: The Long-Document Transformer. arXiv preprint arXiv:2004.05150.
