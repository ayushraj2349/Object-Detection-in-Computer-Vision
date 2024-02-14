# Description

The .ipynb file is the Colab Notebook with all the necessary code.

best.pt is the best model achieved by training the YOLOv8 model.

precision_recall_results_RCNN stores the results of *Precision & Recall* for each class in a dictionary.

mAP_value_RCNN is stored here to compare the 2 Models YOLOv8 & Faster R-CNN.

labels gives you visualization of the how the dataset looks like in terms of occurrencs of each class.

results gives you the results logged of every epoch trained for 20 epochs.

test_results-20240211T212003Z-001 is a zip file containing all the necessary test results and predictions for evaluation and inference.

args.yaml file stores all the hyperparameter values & configurations used in training of YOLOv8 Medium Version Model.

default.yaml files stores the default values initially, if not altered, they'll be used for training.

## as it can be used on **VIDEOS**, the same we've applied and gotten the results.

videos_infer contains all the sample videos used for predicition

video_infer_results contains all the predictions on those sample videos.
