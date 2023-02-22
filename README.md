# recommender_system_flickr
Recommender models from Flickr dataset

The **user-item interaction data** is the main data. This data is further split into training, validation, and test sets.

**Training data**. The training dataset contains a set of interactions between users and items (photos). If a user liked a photo (e.g., click the "heart" emoji which indicates a positive engagement), then there will be a record in the dataset.<br>
**Test data**. Each user is provided with a list of 100 candidate photos in the test dataset, we want to check the candidate list and recommend the top 15 photos for each user. This file was used for a Kaggle competition, to rank models, but here the ground truth is hidden.<br>
**Validation data**. A validation dataset to tune the model. The dataset format is similar to the Test dataset, except that the ground truth of the rating is given.

In addition to the interaction data (training data):

**Item information**. Each photo is represented as a 256-dimensional embedding which is extracted from a pre-training deep learning framework.<br>
**User information**. Each user is represented as a 256-dimensional feature representation, which is the average of the image feature representations she liked in the training data<br>
**Social information**. If two users are friends, there will be a link between two users.
