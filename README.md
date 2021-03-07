# LAB TASK - 4 :

## Layout of The Project - 
  
  The Lab-project consists of a main folder named as 19074005-Dhruv-Gupta which consists of three sub-folders –
  
   1) **Chunking** – 
         
         o Chunking_RNN – 
            
            *	Chunking_RNN.ipynb
            
            *	Chunking_RNN_model.pb
         
         o	Chunking_Bi-LSTM –
           
            *	Chunking_Bi-LSTM.ipynb
            
            *	Chunking_Bi-LSTM_model.pb

   2)	**NER** – 
       
        o	NER_RNN – 
            
            *	NER_RNN.ipynb
            
            *	NER_RNN_model.pb

        o *NER_Bi-LSTM* – 
            
            *	NER_Bi-LSTM.ipynb
            
            *	NER_Bi-LSTM_model.pb

   3)	**POS_tagging** – 
   
   o POS_tagging_RNN – 
            
            *	POS_tagging_RNN.ipynb
            
            *	POS_tagging_RNN_model.pb
       
  o POS_tagging_Bi-LSTM –
            
            *	POS_tagging_Bi-LSTM.ipynb
            
            *	POS_tagging_Bi-LSTM_model.pb

  =>	Google-Colab notebook (.ipynb) – It consists of the whole code which trains and test the data.
  
  =>	Model trained (.pb) – It consists of the model trained i.e., RNN or Bi-LSTM.
  

## Chunking:

Chunking refers to the process of taking individual pieces of information and grouping them into larger units.

### Implementation:

First, we import all necessary libraries and download conll2000 dataset:

* Step 1: Process the dataset and categorise the data into words (x) and chunk_tags(y) and
          splitted the data into training , testing , validation sets.

* Step 2: Implemented both the RNN and Bi-LSTM models using libraries and plotted their results and 
          finally we visualized and compared individual models.
          
* Step 3: Fially, compared the results of these model with the CRF++ models and finally summarised them.

### Results:

- In Chunking, using RNN we got 98.44% accuracy and using Bi-lstm we got 98.14% accuracy.

## POS Tagging:

POS tagging is the process of classifying words into their part of speech and labelling them accrodingly is called POS tagging.
Here, we have tried to implement it using RNN (Recurrent Neural netwrork) and Bi-lstm (Bi directional Lstm)

### Implementation:

First, we import all necessary libraries and download conll2000 dataset:

* Step 1: Process the dataset and categorise the data into words (x) and tags(y) and
          splitted the data into training , testing , validation sets.

* Step 2: Implemented both the RNN and Bi-LSTM models using libraries and plotted their results and 
          finally we visualized and compared individual models.
          
* Step 3: Finally, compared the results of these model with the CRF++ models and finally summarised them.

### Results:

- POS tagging using RNN we get 99.09% accuracy and using Bi-lstm we get 99.34% accuracy.

## NER:

NER (Named Entity recognition) is a task of information extraction that seeks to locate and classify named enitties mentioned in unstructured texts into pre-defined categories such as name of a person, locations , quantities , measurments etc.

Here, we have tried to implement it using RNN (Recurrent Neural netwrork) and Bi-lstm (Bi directional Lstm).

### Implementation:

First, we import all necessary libraries and download conll2000 dataset:

* Step 1: Process the dataset and categorise the data into words (x) and tags(y) and
          splitted the data into training , testing , validation sets.

* Step 2: Implemented both the RNN and Bi-LSTM models using libraries and plotted their results and 
          finally we visualized and compared individual models.
          
* Step 3: Finally, compared the results of these model with the CRF++ models and finally summarised them.

### Results:

- NER, using RNN we get 99.54% accuracy and using Bi-lstm we get 97.11% accuracy.

## RNN -

* Recurrent neural network (RNN) is a neural network that is suitable for modeling sequential information. Although theoretically it is able to capture long-distance             dependencies, in practice it suffers from the gradient vanishing/exploding problems.

* RNN recalls the past and its selections are motivated with the aid of what it has learned from the past.

### Advantages - 

* The principal advantage of RNN is that RNN can model a collection of records (i.e. time collection) so that each pattern can be assumed to be dependent on previous ones.

* Recurrent neural networks are even used with convolutional layers to extend the powerful pixel neighbourhood.

## Bi- LSTM -

 * Bidirectional recurrent neural networks(RNN) are really just putting two independent RNNs together. This structure allows the networks to have both backward and forward   information about the sequence at every time step.

 * Using bidirectional will run our inputs in two ways, one from past to future and one from future to past and what differs this approach from unidirectional is that in the LSTM that runs backward, we preserve information from the future and using the two hidden states combined you are able in any point in time to preserve information from both past and future.
 
 ### Advantages -
 
 * It solves the problem of fixed sequence to sequence prediction.
  
## Conclusion: 

-In all three of the above, i.e. POS Tagging, Chunking, NER, we got very high accuracy using Bi-LSTM and RNN when compared with CRF++ implementation. 

Using CRF++, we got the accuracies as follows:

* Chunking : 94-96%

* NER : 84-85%

* POS_Tagging : 93-94%

### We can conclude that our present accuracies using Bi-LSTM and RNN are far better than the ones using CRF++.
