# spotify-MPD-recommendation
Data source: https://www.aicrowd.com/challenges/spotify-million-playlist-dataset-challenge

How to run:
●	KMeans Instruction to train KMeans model 
○	Download and unzip the file
○	Place the unzipped folder inside this directory
○	Install all required python libraries with pip
■	Pandas
■	Numpy
■	Scipy
■	Matplotlib
■	Nltk
■	Wordcloud
■	Stop_words
■	Gensim
■	Pickle
■	Sklearn
■	yellowbrick
○	Run kmeans_model_final.ipynb 
○	The run time for using 1 JSON file as raw data is about 6 hours (If you want to train the model with more data, you can change the variable number_of_json_file.)

●	KMeans Instruction to use Recommender System
○	Install all required python libraries with pip
■	Pandas
■	numpy 
■	pickle
○	Make sure the kmeans_model_nlp.sav located in the same directory as recommender_system.ipynb
○	Run recommender_system.ipynb
○	Change the artist name and track name or recommended size if you want (NOTE: case sensitive)

●	KMeans evaluation analysis
○	Redefine the variables ‘tracks_data’, ‘test_tracks_data’, ‘Model’ in evaluation notebook‘recommender_system._eval.ipynb’
○	Using TensorFlow API ‘tf.keras.models.load_model’ to load the model.
○	The saved model  named ‘kmeans_mode_nlp.sav’, can be directly imported and used to predict.
○	The saved dataset  named “preprocessed_test_dataset.csv”, can be directly imported and used as ‘tracks_data’ variable.
○	The saved train data set  named “trial.csv”, can be directly imported and used as ‘test_tracks_data’ variable.
○	Then, run the notebook, ‘VG16_fea_reduc.ipynb’ line by line.

●	Word2Vec
○	All code is saved in ‘final_submission/code/word2vec/song2vec.ipynb’ file.
○	The preprocessed dataset for train and test has been saved as ‘train_10000.txt’, and ‘test_10000.txt’.
○	The ‘text_line_reader’ is used to load the train and test txt files.
○	The trained model has been saved as ‘w2v_10k_final’.
○	Genism model load API ‘models.Word2Vec.load()’ is used to load the model.
○	If you want to check the whole process of the project, you can run the notebook line by line.
