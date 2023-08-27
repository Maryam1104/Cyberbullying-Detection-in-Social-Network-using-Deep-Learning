# Cyberbullying-Detection-in-Social-Network-using-Deep-Learning
Lond Short-Term Memory (LSTM) has been used in this experiment.


In this experiment, the Twitter (microblogging platform) dataset is used. I have downloaded this dataset from Kaggle. This dataset is manually labeled and publicly available. In light of all of this, this dataset contains more than 47000 tweets labeled according to the class of cyberbullying: Age; Ethnicity; Gender; Religion; Other types of cyberbullying, and Not cyberbullying. The data has been balanced in order to contain 8000 of each class. However, my study is based on binary
classification. so I have selected and combined racism and gender-based discrimination tweets altogether and labeled it as a cyberbullying class while the other class is non-cyberbullying. Each class contains 5000 tweets so the data has been balanced. This study focuses on extracting English-language tweets. The data set is divided into testing and training data sets. The model is trained using training data, and it needs test data to calculate its performance metric. The model may then classify the recently created tweets obtained from the Twitter API into cyberbullying and non-cyberbullying categories by doing this.

After the pre-processing of data, I have extracted two sorts of highlights from the dataset, to be specific unigrams and bigrams. Made recurrence dissemination of the unigrams and bigrams present in the dataset and picked the top N unigrams and bigrams for our analysis.

Long Short-Term Memory (LSTM) has been used in this experiment. A fixed-length sequence of words is processed by the model’s
embedding layer. To prevent overfitting, there are two dropout layers that are used: one before the neural architecture layer (with dropout rates of 0.25) and one after (with dropout rates of 0.5). The fully connected layer follows, and it is a dense output layer with an equal number of neurons in each class. The softmax layer, which offers softmax activation, is the bottom layer. Backpropagation using the Adam optimizer and the categorical cross-entropy loss function is used to train all the models.
