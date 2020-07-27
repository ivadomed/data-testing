# data-testing
Light-weighted data for testing/tutorial

# Content
model\_unet.pt --> .pt file for inference testing

sub-unf01 --> Bids folder with multiple contrast (T2w,T2star and T1w). Original image from https://github.com/ivadomed/data\_example\_spinegeneric/releases/tag/r20200907 resampled to 1mm isotropic and converted to float32

derivatives/labels/sub-unf01 --> derivatives folder with seg-manual labels for all contrasts (from https://github.com/ivadomed/data\_example\_spinegeneric/releases/tag/r20200907), labels-disc-manual labels for T2w, lesion-manual label for all contrasts, which are manullay created dummy segmentation. All images were resampled to 1mm isotropic and converted to float 32

bounding\_box.json --> dictionnary to test certain function from  ivadomed/scripts/bounding\_box.py

dataset\_description.json --> needed file to descript dataset

participants.csv --> table with subject names and potential metadata

temporary\_results.csv --> Used to test ivadomed/scripts/compare\_models.py
