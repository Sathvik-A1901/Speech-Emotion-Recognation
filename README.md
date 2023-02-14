# Speech-Emotion-Recognation

#DESCRIPTION

The project is all about speech emotion recognation, recognizing emotions like happy,fear,surprise,sad,angry,disgust.Making a computer understand 
our emotions by recognizing our voice would help in our real life senarios like customer care services, Emergency calls,improving features in bots
like alexa,and deploying models in robots make them more interactive with humans.The dataset which we have considered is TESS dataset.The features 
for every emotion included a Mel-frequency cepstral coefficients. This coefficients describes overall shape of spectral envelope. This fretures are
extracted for every voice in the dataset.We have developed a deep learning model and trained the model with those features(coefficients). The model 
which we considered spcifically called as LSTM (Long Short Term Memory) Reccurent Neural Network.It's basically a RNN where its gates in the neurons 
make them stand a part from the acutal RNN. 
              
              
The project underwent few phases in Data Science.
   Phase 1:-
   
      Data Collection:-
      In this phase we have done research on what dataset would be good for our problem statement. We have decided to take TESS(Toronto emotional speech set) data 
      set and work on it. It includes 200 voices of each and every emotion those are of 2 womens.
   
   Phase 2:-
   
      Exploratory Data Analysis:-
      EDA is an approach to analyze the data using visual techniques,we have plotted:
      -->Wave Plot
      -->Spectrogram 
      of different emotions with different modulations
   
   Phase 3:-   
   
   Feature Extraction:
      We can't take the raw audio signal as input to our model because there will be a lot of noise in the audio signal. It is observed that extraction features 
      from the audio signal and using it as input to the base model will produce much better performance than directly considering raw audio signal as input.MFCC is
      the widely used technique for extracting the features from audio signal.
   
   Phase 4:-
          
       Model Building:
       After extracting required features we need to train our model. It is recommended that the prediction of such emotions from these type of features may vary 
       from time to time. More over  we need a model which keeps track of our recent data . There is a RNN varient called LSTM RNN which keeps on track of our past            actions.A traditional RNN has a single hidden state that is passed through time, which can make it difficult for the network to learn long-term dependencies.          LSTMs address this problem by introducing a memory cell, which is a container that can hold information for an extended period of time. The memory cell is              controlled by three gates: the input gate, the forget gate, and the output gate. These gates decide what information to add to, remove from, and output from the        memory cell.
      
#HOW TO RUN CODE
step 1:
extract a voice from running the voice recorder file
step 2:
run the SEP file  in jupyternotebook
at last add your recored file in it and run the cells below it.
