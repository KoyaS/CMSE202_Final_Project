# Final Project: Image Classification, Boat or Not Boat?

## Functions:
- `browse_images`: Takes in image arrays, image labels and label classes. Creates an interactive image plot with a slider allowing user to look through images and their associated labels.
- `browse_predictions`: Similar to browse_images, takes in image arrays, image labels and label classes. However, also takes in a classifier's predictions and displays them alongside the image's true labels.
- `train_SVC`: Takes in training data and its labels in addition to a boolean value indicated whether or not to use grid search. After some time, returns a trained SVC classifier. Also pickle dumps trained classifier to a file called 'best_classifier.p'.
- `section_scene`: Takes in a scene name which is imported from a png. Subdivides a scene into 80x80px sections to match the training data. Does this in a grid pattern. Returns an array of images and their respective xy coordinates on the original scene.
- `mark_predictions`: Takes in sectioned scene, scene section's xy locations, classifier predictions of scene sections and the original scene image. Displays a plot with red squares around sections of the image the classifier has labeled as having a boat.

## Notes:
- Be sure to have all libraries in the imports section installed.
- Our dataset isn't in the repo, see below for more details.

## Dataset:
Since the dataset is so large, we were unable to upload it to github. You will have to pull the project and download the dataset seperately. 
1. Download dataset from the [Kaggle Ships in Satellite Imagery](https://www.kaggle.com/rhammell/ships-in-satellite-imagery 
) page. 
2. Extract the `shipsnet.json` file from the downloaded dataset onto the same level as the `CMSE 202 Final Project.ipynb` file.
3. Discard the rest of the dataset
4. Unzip the `Classifiers.zip` (this zip is in the git repo) and place the Classifiers folder on the same level as the `CMSE 202 Final Project.ipynb` file.
5. Discard the `Classifiers.zip` file.

After doing this our project should run.

# Project Contributions

# Koya: 
- Managed git repo
- Created SVM classifier function
- Created algorithm for breaking scene into sections
- Fitted CNN classifier
- Wrote slides  
# Brett:
- Helped read in data
- Helped tidy and format RGB data
- Set up PCA
- Used SVM to compare PCA accuracy
- Wrote slides
