# data-testing
Light-weighted data for testing/tutorial

# Content
* sub-unf01: BIDS folder with multiple contrast (T2w, T2star and T1w). Original image from [ivadomed spine generic example repo](https://github.com/ivadomed/data_example_spinegeneric/releases/tag/r20200907) resampled to 1mm isotropic and converted to float32 to reduce repo size. Subject was randomly selected among the available subjects. Images are oriented according to RPI convention and were cropped with the following bounding box x=[50, 181], y=[60, 201], z=[10, 26].
* `derivatives/labels/sub-unf01`: derivatives folder with `_seg-manual` segmentations for all contrasts (from [ivadomed spine generic example repo](https://github.com/ivadomed/data_example_spinegeneric/releases/tag/r20200907)), lesion-manual label for all contrasts, which are manullay created dummy segmentation. All images were resampled to 1mm isotropic and converted to float 32. Images are oriented according to RPI convention and were cropped with the following boynding box x=[50, 181], y=[60, 201], z=[10, 26].
* bounding\_box.json: dictionnary to test certain function from  ivadomed/scripts/bounding\_box.py.
* dataset\_description.json: needed file to descript dataset.
* participants.csv: table with subject names and potential metadata. 
* temporary\_results.csv: Used to test ivadomed/scripts/compare\_models.py. 
