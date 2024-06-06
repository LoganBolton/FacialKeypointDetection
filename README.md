# FacialKeypointDetection
Facial Keypoints Detection Kaggle Competition. The objective of this competition is to predict keypoint positions on face images.

[Link to Kaggle Competition](https://www.kaggle.com/competitions/facial-keypoints-detection)

## Approach
For this competition I tried training using a Resnet model, a regular CNN and a CNN with dropout and batch normalization. The Resnet model had slightly performance, but took significantly longer to train and had much longer inference time. To see this model, checkout the resnet branch. The model in the main branch is the CNN with dropout and batch normalization. Check out the Submission part of the notebook for more specific details about training and results.

## Thoughts
The models I trained have significant room for improvement. Most notably, the model is also very sensitive to things like glasses or more unusual face shapes. This suggests that it struggles with generalization and needs either better data or better training techniques to improve further. The data quality could definitely be improved. Adding transformations to the test images could be used to make significantly more training data. Also there is a significant amount of missing data in the training set. I used a simple average to replace that missing data, but more sophisticated techniques would probably work better.  

![plot](./data/images/examples.png)
