# How the term of Attention Mechanism was introduced and What and Why of Attention Mechanism

![image.png](attachment:image.png)



***
### Introduction of seq2seq models and application:

<font color=blue>TextSequence to sequence was first introduced by Google in 2014. So let’s go through our question what is seq2 seq model? Sequence to sequence model tries to map input text with fixed length to output text fixed-length where the length of input and output to the model may differ. As we know variants of Recurrent neural networks like Long short-term memory or Gated Recurrent Neural Network (GRU) are the method we mostly used since they overcome the problem of vanishing gradient.
From the example shown in the image is of language conversion from French to English. </font>


![image.png](attachment:image.png)

<font color=blue>Another example of English to Hindi Translation. Which is nothing but google translation.</font>

 ![image.png](attachment:image.png)

***
## Refrences

Sequence to Sequence Learning with Neural Networks was introduced by 
* Ilya Sutskever Google ilyasu@google.com 
* Oriol Vinyals Google vinyals@google.com 
* Quoc V. Le Google qvl@google.com
* Paper Reference:
* •	 https://papers.nips.cc/paper/5346-sequence-to-sequence-learning-with-neural-networks.pdf
* •	https://arxiv.org/abs/1409.3215


***
## Application of Seq2seq models

1.	Speech Recognition
2.	Machine Language Translation
3.	Name entity/Subject extraction
4.	Relation Classification
5.	Path Query Answering
6.	Speech Generation
7.	Chatbot
8.	Text Summarization
9.  Product Sales Forecasting


![image.png](attachment:image.png) <center>**Seq2Seq is encoder and decoder.**</center> 


![image.png](attachment:image.png)

***
## So why does the seq2seq model fails?

### Details of the architecture and function already explained by my colleagues so now we see where this model lags. 

##### * As we saw encoder takes input and converts it into a fixed-size vector and then the decoder makes a prediction and gives output sequence. It works fine for short sequence but it fails when we have a long sequence because it becomes difficult for the encoder to memorize the entire sequence into a fixed-sized vector and to compress all the contextual information from the sequence. As we observed that as the sequence size increases model performance starts getting degrading.

***
### <font color = Dark Green>**How can we overcome the problem of long sentences and performance of the model?</font>
***

****
## Here comes the solution with Attention Mechanism

As the word ‘attention’ suggest importance is given to specific part of context while so as to increase the performance and output interpretation is starts to make sense. In simple terms we give importance to specific parts of the sequence instead of the entire sequence predict that word. Basically, in the attention, we don’t throw away the intermediate from the encoder state but we utilize this to generate context vector from all states so that the decoder gives output result.
*	The attention mechanism has changed the way we work with deep learning algorithms
*	Fields like Natural Language Processing (NLP) and even Computer Vision have been revolutionized by the attention mechanism
![image.png](attachment:image.png)

**For Example:** For Deep learning we have to read an article and get the inference out it. Or a whole book. Like the human brain attention is given to specific words which mind interprets and grasps others are just a blurry information. 

### <center> <font color = blue>Text Attention</font> <center>  

![image.png](attachment:image.png)

### <center> <font color = blue> Image Attention

![image.png](attachment:image.png)

### 'So, whenever the proposed model generates a sentence, it searches for a set of positions in the encoder hidden states where the most relevant information is available. This idea is called ‘Attention’.'

****
## How it Works

![image.png](attachment:image.png)

![image.png](attachment:image.png)

![image.png](attachment:image.png)

***
## Attention Unit

![image.png](attachment:image.png)

### Types of Attention

![image.png](attachment:image.png)

#### <font color = blue>1.Soft Attention</font>

![image.png](attachment:image.png)

#### <font color= blue>2. Hard Attention1

![image.png](attachment:image.png)

***
### <font color = blue>Architecture of Attention Model

![image.png](attachment:image.png)

***

![image.png](attachment:image.png)

![image.png](attachment:image.png)

![image.png](attachment:image.png)

***
## <font color = blue>Drawbacks:

#### <font color =Red>Only one drawback of attention is that it’s time-consuming. To overcome this problem Google introduced <font color=Green>“Transformer Model” .'

![image.png](attachment:image.png)


```python

```
