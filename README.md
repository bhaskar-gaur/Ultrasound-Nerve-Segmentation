# Ultrasound-Nerve-Segmentation

## Goal:
**Identify nerve structures in ultrasound images of the neck**

   The task in this competition is to segment a collection of nerves called the Brachial Plexus (BP) in ultrasound images. You are provided with a large training set of images where the nerve has been manually annotated by humans. Annotators were trained by experts and instructed to annotate images where they felt confident about the existence of the BP landmark.

## Source:
https://www.kaggle.com/c/ultrasound-nerve-segmentation/

## Important Points:
- The dataset contains images where the BP is not present. Your algorithm should predict no pixel values in these cases.
- As with all human-labeled data, you should expect to find noise, artifacts, and potential mistakes in the ground truth. Any individual mistakes (not affecting the broader integrity of the competition) will be left as is.
- Due to the way the acquisition machine generates image frames, you may find identical images or very similar images.
- In order to reduce the submission file sizes, this competition uses run-length encoding (RLE) on the pixel values. The details of how to use RLE are described on the 'Evaluation' page.

## File descriptions:
- **/train/** contains the training set images, named according to subject_imageNum.tif. Every image with the same subject number comes from the same person. This folder also includes binary mask images showing the BP segmentations.
- **/test/** contains the test set images, named according to imageNum.tif. You must predict the BP segmentation for these images and are not provided a subject number. There is no overlap between the subjects in the training and test sets.
- **train_masks.csv** gives the training image masks in run-length encoded format. This is provided as a convenience to demonstrate how to turn image masks into encoded text values for submission.
- **sample_submission.csv** shows the correct submission file format.



