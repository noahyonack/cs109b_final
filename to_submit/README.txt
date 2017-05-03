SCREENCAST YOUTUBE LINK: www.youtube.com/link-here

This is a README that goes with the notebooks. It explains how much the notebooks changed since the milestone submissions. This is to guide the TF to find relevant updates.

Since the last milestone, we've since refactored much of our code to make sure it's readable, modular, and easy for the TF to examine.

Here's a list of all the notebooks we're submitting as well as a description of what each one contains.

1. milestones_1_2.ipynb

This notebook contains our data collection and scraping from both Milestone 1 and Milestone 2. Nothing has changed in this notebook since the submission because all we're doing is scraping the TMDB API and processing our data into a dataframe. 

2. Milestone_3_Lasso_RandomForest_Section.ipynb

This notebook contains our *updated* code for Milestone 3, which we ended up changing a lot since the submission. We originally submitted an incomplete notebook due to last-minute issues with merge conflicts and unforsoon data processing bugs, but we've since changed this notebook to contain two different models: a LASSO linear regression (which ended up performing terribly in predicting genre) and a Random Forest (which ended up doing well). 

3. PreMilestone4DataCleaning.ipynb

Because Milestone 4 (deep learning) was so complicated, we decided to refactor our code so that it's easier to follow. This notebook contains much of the data cleaning and processing for milestone 4. In this notebook, we collapsed all 19 genres into 3 more general categories so that our label matrix (y_train) would be more dense. We also write code to download and manipulate our images by size (32x32 or 64x64) and color (RGB or grayscale). 

All the images we manipulate are saved locally and uploaded as part of the final submission.

4. cnn_from_scratch.ipynb

This is *similar* to the first part of Milestone 4, but it is more modular and more rigorous. It uses the data that we created in PreMilestone4DataCleaning.ipynb. It takes the two best models from Milestone 4 (model 1 and model 3) and tries out various combinations of image size and color. It ignores the 3 other models that we tried in milestone 4 but found to be poor performing. We included the descriptions of these models in the bottom of this notebook, though we don't include the code for running these models because they are poorly performing and the code can already be found in Milestone 4.

5. pretrained_cnn.ipynb

This is the same as the second part of Milestone 4. It contains the code we used to re-train a pre-trained model. We have not changed the code in this notebook because it was well done from the start. 

6. Rnn+on+Text.ipynb

This notebook is totally new (not found in other milestones), and it contains code that we wrote to build a recurrent neural network (RNN) to predict genre based on text data (such as movie plots and actor names).

Our data can be found in data.zip. It contains our two datasets (one has 19 genres and the other is an exact copy with just 3 more general genre categories). data.zip also contains a directory called final_imgs_folder/, which contains all versions of images that we fed through our neural networks (e.g. rgb images of size 32x32, grayscale images of size 64x64, etc.)
