# data-testing
Light-weighted data for testing/tutorial

# Content
* sub-unf01: BIDS folder with multiple contrast (T2w, T2star and T1w). Original image from [ivadomed spine generic example repo](https://github.com/ivadomed/data_example_spinegeneric/releases/tag/r20200907) resampled to 1mm isotropic and converted to float32 to reduce repo size. Subject was randomly selected among the available subjects. Images are oriented according to RPI convention and were cropped with the following bounding box x=[50, 181], y=[60, 201], z=[10, 26].
* `derivatives/labels/sub-unf01`: derivatives folder with the following labels:
  * `_seg-manual`: spina cord segmentations for all contrasts,
	* `_lesion-manual`: dummy labels which are supposed to represent lesion segmentation. WARNING: these are *not* actual lesion segmentations, but are only here for the purpose of testing the workflow of `ivadomed` codebase.
  * `_labels-disc-manual`: dummy label (single voxel), which is supposed to represent disc label. WARNING: this is *not* an actual label that represent the anatomy, but is only here for the purpose of testing the workflow of `ivadomed` codebase.

All images were resampled at 1mm isotropic and converted to Float32. Images were oriented according to RPI convention and were cropped with the following bounding box: x=[50, 181], y=[60, 201], z=[10, 26].
* bounding\_box.json: dictionary to test a specific function from `ivadomed/scripts/bounding_box.py`.
* dataset\_description.json: this file is needed to described the dataset.
* participants.csv: table with subject name and potential metadata.
* temporary\_results.csv: Used to test `ivadomed/scripts/compare_models.py`.
