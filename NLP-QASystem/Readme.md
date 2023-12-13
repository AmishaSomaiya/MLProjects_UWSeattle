Question answering is a reading comprehension task, one of the most prevalent research problems in NLP. It takes 2 inputs : the passage which can be one or more paragraphs and the query which is the question posed by the user. The output is the response to the question, single word or longer and is a substring of the passage which is most contextually relevant to the question. This project implements a closed-domain, extractive Question Answering system using NLP with SQuAD using 2 traditional ML and 2 DL approaches. The traditional ML approaches Multinomial Logistic Regression and Random Forest use hand-crafted features only and hence are unable to correctly comprehend the complex linguistic patterns and are unable to correctly capture the contextual understanding of words and phrases leading to low scores. The third model implementation uses pre-trained BERT and achieves F1 : 88.7 and EM : 85.4 high scores because BERT being based on the Transformer architecture, understands context from entire input sequence and not just a fixed window. Also, BERT is pre-trained on a large corpus using unsupervised learning which helps it learn complex contextual patterns easily. However, BERT is a large model with 340 million parameters and hence becomes impractical to users with limited resources. Thus, the final project implementation is ‘DistilBERT backbone + additional head : trained from scratch’ which retains the first few layers of DistilBERT backbone and then with an additional head with 3 layers, the model is trained specifically for QA task. This final implementation achieves F1 : 84.56 and EM : 75.846 which is comparable to BERT in just 3 epochs while at the same time having 40% lesser parameters, light weight and computationally efficient. 