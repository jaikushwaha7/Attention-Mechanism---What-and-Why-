# How the term of Attention Mechanism was introduced and What and Why of Attention Mechanism

<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img1.png" />



## Topics Covered

**[1.<a href="1.Introduction-of-seq2seq-models-and-application">Introduction-of-seq2seq-models-and-application</a>]**
2. <a href="#2.References">References</a>
3. <a href="#3.Application-of-Seq2seq-models">Application of Seq2seq models</a>
4. <a href="#4.Basic-Structure-of-Seq2Seq-as-encoder-and-decoder.">Basic Structure of Seq2Seq as encoder and decoder.</a>
5. <a href="#5.So-why-does-the-seq2seq-model-fails?">So why does the seq2seq model fails?</a>
6. <a href="#6.Here-comes-the-solution-with-Attention-Mechanism">Here comes the solution with Attention Mechanism</a>
7. <a href="#7.How-it-Works">How it Works</a>
8. <a href="#8.Attention-Unit">Attention Unit</a>
9. <a href="#9.Types-of-Attention">Types of Attention</a>
10. <a href="#10.Architecture-of-Attention-Model">Architecture of Attention Model</a>
11. <a href="#11.Application-of-Attention-Model">Application of Attention Model</a>
12. <a href="#12.Drawbacks:">Drawbacks</a>
13. <a href="#13.Summary:">Summary</a>

***
### 1.Introduction of seq2seq models and application<a name="1.Introduction of seq2seq models and application"></a>

<font >TextSequence to sequence was first introduced by Google in 2014. So let’s go through our question what is seq2 seq model? Sequence to sequence model tries to map input text with fixed length to output text fixed-length where the length of input and output to the model may differ. As we know variants of Recurrent neural networks like Long short-term memory or Gated Recurrent Neural Network (GRU) are the method we mostly used since they overcome the problem of vanishing gradient.
***From the example shown in the image is of language conversion from French to English.*** </font>
<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img2_1.png" />


<font color=blue>Another example of English to Hindi Translation. Which is nothing but google translation.</font>
<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img3_1.png" />


[<a href="#Topics-Covered">Back to Top</a>]

***
## 2.References

Sequence to Sequence Learning with Neural Networks was introduced by 
* Ilya Sutskever Google ilyasu@google.com 
* Oriol Vinyals Google vinyals@google.com 
* Quoc V. Le Google qvl@google.com
* Paper Reference:
* •	 https://papers.nips.cc/paper/5346-sequence-to-sequence-learning-with-neural-networks.pdf
* •	https://arxiv.org/abs/1409.3215


[<a href="#Topics-Covered">Back to Top</a>]

***
## 3.Application of Seq2seq models

1.	Speech Recognition
2.	Machine Language Translation
3.	Name entity/Subject extraction
4.	Relation Classification
5.	Path Query Answering
6.	Speech Generation
7.	Chatbot
8.	Text Summarization
9.  Product Sales Forecasting


[<a href="#Topics-Covered">Back to Top</a>]

### 4.Basic Structure of Seq2Seq as encoder and decoder.
<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img5.png" />



### <center>Seq2Seq is encoder and decoder.
<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img4.png" />


***
## 5.So why does the seq2seq model fails?

###  As the Details of the architecture and function already explained by my colleagues so now we see where this model lags. 

#### As we saw encoder takes input and converts it into a fixed-size vector and then the decoder makes a prediction and gives output sequence. It works fine for short sequence but it fails when we have a long sequence because it becomes difficult for the encoder to memorize the entire sequence into a fixed-sized vector and to compress all the contextual information from the sequence. As we observed that as the sequence size increases model performance starts getting degrading.


***
### <font color = Dark Green>**How can we overcome the problem of long sentences and performance of the model?</font>
***

[<a href="#Topics-Covered">Back to Top</a>]

****
## 6.Here comes the solution with Attention Mechanism

As the word ‘attention’ suggest importance is given to specific part of context while so as to increase the performance and output interpretation is starts to make sense. In simple terms we give importance to specific parts of the sequence instead of the entire sequence predict that word. Basically, in the attention, we don’t throw away the intermediate from the encoder state but we utilize this to generate context vector from all states so that the decoder gives output result.
*	The attention mechanism has changed the way we work with deep learning algorithms
*	Fields like Natural Language Processing (NLP) and even Computer Vision have been revolutionized by the attention mechanism
<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img6.png" />


**For Example:** For Deep learning we have to read an article and get the inference out it. Or a whole book. Like the human brain attention is given to specific words which mind interprets and grasps others are just a blurry information. 

### <center> <font color = blue>Text Attention</font> <center>  
<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img7.png" />


### <center> <font color = blue> Image Attention
<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img8.png" />


### 'So, whenever the proposed model generates a sentence, it searches for a set of positions in the encoder hidden states where the most relevant information is available. This idea is called ‘Attention’.'

[<a href="#Topics-Covered">Back to Top</a>]

****
## 7.How it Works
<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img9.png" />

<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img10.png" />

<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img11.png" />


[<a href="#Topics-Covered">Back to Top</a>]

***
## 8.Attention Unit
<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img12.png" />


[<a href="#Topics-Covered">Back to Top</a>]

### 9.Types of Attention
<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img13.png" />


### <font color = blue>* Lets have a look at Soft Attention on computer vision</font>
<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img14.png" />


### <font color= blue> Hard Attention on Computer Vision
<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img15.png" />


[<a href="#Topics-Covered">Back to Top</a>]

***
### <font color = blue>10.Architecture of Attention Model
<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img16.png" />


***

[<a href="#Topics-Covered">Back to Top</a>]

***
### <font color = blue>11.Application of Attention Model
<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img17_1.png" />

<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img18.png" />

<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img19.png" />


[<a href="#Topics-Covered">Back to Top</a>]

***
## <font color = blue>12.Drawbacks:

The main disadvantage of the **attention mechanism is that it adds more weight parameters to the model**, which can increase training time especially if the input data for the model are long sequences.

In a sequence-to-sequence model (e.g. RNN-based encoder-decoder), the attention mechanism combines the encoder’s output at each time step, along with the decoder’s output at time step t, to create the context vector for time step t. The context vector encapsulates the most relevant information from the encoder, which is why attention is a useful mechanism.

However, in calculating the context vector we use trainable weights for each of the encoder’s time steps.**This can be a very large number of weight parameters if the input data for the encoder is long, which is the case in tasks like text summarization. And the larger a model gets (in terms of number of parameters), the longer it takes to train.**

***
#### <font color =Red>So the only one drawback of attention is that it’s time-consuming. To overcome this problem Google introduced <font color=Green>“Transformer Model” .'
***

[<a href="#Topics-Covered">Back to Top</a>]

***
## <font color = blue>13.Summary:
<img src="https://github.com/jaikushwaha7/Attention-Mechanism---What-and-Why-/blob/main/img20_1.png" />


There are many variants in the cutting-edge researches, and they basically differ in the choice of soft attention and hard attention.
***As, attention mechanism is very actively researched nowadays and it is expected that there will be more and more domains welcoming the application of attentional models.***

[<a href="#Topics-Covered">Back to Top</a>]


:+1: :sparkles: :camel: :tada:
:rocket: :metal: :octocat: 


```python

```
