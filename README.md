**SImple Titanic NN**

This repo contains a jupyter notebook and 3 csv files with the train/test data and results from Kaggle's Titanic challenge

The notebook is my first attempt at applying a Neural Net to a kaggle comp. I know using a Neural Net on a small dataset like Titanic's (~820 exmaples)
is probably overkill, you could get much better results using a gradient boosting algo like XGBoost or just an ensemble method with simpler-than-nn algos.
This notebook is the beginning of the documentation of how I'm going about learning PyTorch. I'm just about finished with the Deep Learning Specialization
course by Andrew Ng so I figured I should start applying my knowledge. If you have taken any DeepLearning.ai courses you might be confused as to why I'm using
PyTorch as opposed to TensorFlow, which is the option mainly used in the courses; it's because in practice, many AI applications are written in PyTorch, 
at least from what I have seen and read online. 

You could definitley improve this model by using more advanced feature engineering or by using a validation set and choosing the best run of the params to
make final predictions. But, I chose not to spend time optimizing a nn on a task where it's overkill in the first place and just move on to another, larger
dataset to fit.

You'll notice that I removed the name column and did a little feature engineering on filling in blank ages, convertong cabins to numbers, etc...
Ages - I filled the blank age cells with the median age from their corresponding Pclass and Sex
Cabin - I assigned numerical values to the cabins based on height/closeness to the top of the ship
Ticket - I just removed the letters from the original ticket num column
Sex - Changed male and female to binary 1 or 0

Note: I'm aware this feature engineering strategy may not be the most optimal, but, it allows me to build and run the model on the data, which is what I care
about, not the results.

Feel free to build off of this model and experiment further!


**Built without AI**
