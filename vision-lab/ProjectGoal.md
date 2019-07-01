# Object Detection
To find ships in the open sea via satellite images.

# Datasets
- Database of images of tankers, commercial ships, or fishing ships: https://www.kaggle.com/c/airbus-ship-detection/data
- ground truth training images: train_ship_segmentations.csv
- test images (large scale SPOT images at 1.5 m. resolution): sample_submission


# Modeling Strategy
- train a model to learn how to segment an image

- Remove noise from the original image and only consider a “mask” or minimal representation of the image. This “mask” (center image below) is what they were predicting as an output using ML
- Draw a bounding box around the predicted mask

# End Product Goals
aim : locate ships in images, and put an aligned bounding box segment around the ships located.
a model that segments an image?
