# Crop_EM_to_bbox
Run the scripts in order and make sure to follow naming conventions used in the scripts. \n
01 will use the segmentation data, mask not segmented pixels and save the masked images.\n
02 will stitch planes of segmentation data, run 4x4 connectivity analysis and save bounding boxes of found connected areas to a txt file. Current size threshold is 1000px for an area to be detected as object and have its bbox saved.\n
03a or 03b will load the bbox txt, restitch planes of to-be-cropped data crop out the ROIs and save files with coordinates in the names.\n
# CAUTION (Subject to change)
03a and 03b mess up coordinates in the file name, here X is Y and vice versa.\n
03b has a switch in the 'crop_and_save_region' fun which is not implemented c orrectly as of now.\n
