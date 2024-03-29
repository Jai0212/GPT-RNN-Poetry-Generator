# GPT-RNN Poetry Generator

Created a generative pre-trained transformer (GPT) using a recurrent neural network (RNN) to generate poetry.  

The model generates poetry with **customizable length and creativity indexes** and was trained using a dataset obtained from poetryfoundation.org.

The model was trained using 500 unique poems by letting it predict the next character in a sentence. It utilizes long 
short-term memory networks (an RNN) and NLP techniques to improve its generation. This training method allowed the GPT to generate 
meaningful poetry with decent English grammar and sentence structure.

**Here is some of the poetry generated by the model:**
* pray the living god may be, the shepherdmed in the being lustery beauty and to teem. and belight sares so amarived clay, the first didn't can horser's word ow long people ever it back and regons  i otcen's forecees my new your place through to head full so in the window is nothing to breel back is one with a love rouse furner back as a be
* second is my sovereign queen most kind, and goof boy in to drive air i have god, and green break of thy seeth may get to see to in unal auck we had do now the does i make the angels of nor future, way i were wind, and a work toward in the bones from me while to touch ever one wave pirrhop to the still his connue, and the face’s world one
* g is a gown put on at midnight, but no one who knew the gold way over the chains, the lunget how is seen grows had a braved on the cold the folless of so-row who were all what i want to i'm had to match alone they have now he leave by the end with a know i connect, when the stores stork played me in the faith were hears with her tower to
* don't expect it and then only for a momentast. the same. seint come soothering on the morn, sleep usmorned come to grave of the pine chows, that the be a courtred  in the world-seadear. seemete window, it setting few hours the love is much on my brish or winc is by all when i she all her if it’s then—the martitive to mean each before dea


## Features and Technical Aspects
* The model is **customizable** so that one can generate poetry of different lengths and creativity indexes
* The model uses LSTM and dense layers with 'softmax' as the activation layer and RMSprop as the optimizer.  
* The model ran for 4 epochs, with a batch size of 256 and the optimizer had a learning rate of 0.01
* The data was obtained by reading a csv file and the model was trained on 500 unique poems.

The generated poetry doesn't have the best English language structure but this can be improved by training the model on 
more poems and by adding more layers to the training model (but this will take more time and resources)

The entire project was created in Python (3.11) on Pycharm.  

The packages/dependencies used were
* TensorFlow
* NumPy
* Pandas


## Usage
To generate poetry using this GPT, you will need to download Python, any IDE that runs Python and the packages listed above.  

After that, you just need to run the 'poetry_generator.py' file. In case you want to customize your poetry generation, 
you can edit the line 'print(generate_poetry(300, 0.2))' in the same file (line 47). 

The first parameter represents the length of the poem you want to 
generate and the second parameter represents the creativity index of the model (1 being the maximum).  

The dataset is in the directory 'data'.  

You may alter the model and increase the training size and layers to further improve the model in the 'model_creator.py' file.  
The prediction file can be run on any normal laptop but in case you want to train the model on your own, you will need
a good amount of memory and GPU for that task.


## Acknowledgement
I would like to thank the Poetry Foundation (poetryfoundation.org) for providing the dataset that was used in this project. The exact file was downloaded from https://www.kaggle.com/datasets/johnhallman/complete-poetryfoundationorg-dataset?resource=download

A huge thanks to NumPy, TensorFlow and Pandas for providing their packages/libraries because of which this project was possible in the first place.

I worked on this project alone and will not be actively working on this project anymore (I will be creating other related projects). However, I would love any suggestions/feedback/collaborative requests.

##  Author and Date
by Jai Joshi  
25th February, 2024
