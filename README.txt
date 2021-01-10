Name: Becca Dura
Email: dura0083@umn.edu


Files:
-Final_Report.pdf: Contains the final project report with an analysis and comparison of each model.
-Preprocessing.ipynb: This file preprocesses the data for the collaborative filtering models by creating a new subsetted dataset as well as datasets containing ratings from each user for each movie in a matrix and similarity scores between users.
-PM_Basic.ipynb: This file creates the basic popularity method model.
-PM_Weighted.ipynb: This file creates the popularity method model using weighted averaged ratings.
-CB_Genres.ipynb: This file creates the content-based method model using the genres.
-CB_MovieOverview.ipynb: This file creates the content-based method model using the movie overviews/summaries.
-CF_MemoryBasedModel.ipynb: This file creates the collaborative filtering memory-based model, which uses the k-nearest-neighbors algorithm.
-CF_NeuralNetworkBasic.ipynb: This file creates the collaborative filtering model-based model, which uses a basic neural network.
-CF_NeuralNetworkEmbedding.ipynb: This file creates the collaborative filtering model-based model, which uses a neural network with embedding layers.
-CF_SVD.ipynb: This file creates the collaborative filtering hybrid model, which uses SVD (singular value decomposition).


Datasets:
-ml-25m/movies.csv: This dataset contains information for each movie and each movie's ID.
-ml-25m/ratings.csv: This dataset contains the ratings for each movie and user as well as timestamps for the ratings.
-movies_metadata.csv: This dataset contains the metadata for each movie, including the movie overviews and genres.
-new_movies.csv: This dataset is created in the pre-processing file.  It subsets the dataset and relabels the movie IDs and user IDs so they start at zero.
-users.csv: This dataset is created in the pre-processing file.  It contains a large dataframe of ratings by each user for each movie
-users_similarity.csv: This dataset is created in the pre-processing file.  It contains the similarity scores for each combination of users.
-cache.hdf5: This is the cache for the h5py file containing the initial array used to create the "users.csv" file.  It is created in the pre-processing file.
cache.hdf52: This is the cache for the h5py file containing the initial array used to create the "users_similarity.csv" file.  It is created in the pre-processing file.


Instructions to Run Code:
1. Ensure you have the libraries listed in the assumptions installed.
2. Ensure you are using the correct version of python (listed in the assumptions).
3. Open the folder in jupyter notebooks from the command line.  To do this, you should navigate to this folder using the command line and open jupyter notebooks using the following command "jupyter notebook".  If you do not have jupyter notebooks installed on your computer, follow the instuctions in the notes below.
4. Open each file individually to run them.  The datasets are already in the correct locations in the folder to be imported.  The files do not need to be run in any specific order since I already ran "Preprocessing.ipynb" to create the subsetted datasets.  However, if you want to run "Preprocessing.ipynb" yourself, you will first need to delete the following (which are created in the preprocessing python script) from the folder: "new_movies.csv", "users.csv", "users_similarity.csv", "cache.hdf5", and "cache.hdf52".


Assumptions:
1. At least Python 3.6 must be used to run the code.
2. The following libraries must be installed in order for the code to run: numpy, matplotlib, pandas, sklearn, h5py, tensorflow (2.0 or above), and surprise.


Notes:
1. These files are set up as Python notebooks so you can more easily view the recommended movies from the systems and see where specific results come from in the code.
2. The best way to run these files is by opening the entire folder using jupyter notebook from the command line.  If you do not have jupyter notebook installed on your computer, you can find instructions on how to do so at the following website: https://jupyter.org/install.  However, you can also upload the entire folder to Google Drive and run everything in Google Colab if that is easier for you.
