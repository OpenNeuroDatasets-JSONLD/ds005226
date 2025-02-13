**Summary**

In everyday environments, partially occluded objects are more common than fully visible ones. Despite their visual incompleteness, the human brain can reconstruct these objects to form coherent perceptual representations, a phenomenon referred to as amodal completion. However, current computer vision systems still struggle to accurately infer the hidden portions of occluded objects. While the neural mechanisms underlying amodal completion have been partially explored, existing findings often lack consistency, likely due to limited sample sizes and varied stimulus materials. To address these gaps, we introduce a novel fMRI dataset,the Occluded Image Interpretation Dataset (OIID), which captures human perception during image interpretation under different levels of occlusion. This dataset includes  fMRI responses and behavioral data from 65 participants. The OIID enables researchers to identify the brain regions involved in processing occluded images and examines individual differences in functional responses. Our work contributes to a deeper understanding of how the human brain interprets incomplete visual information and offers valuable insights for advancing both theoretical research and related practical applications in amodal completion fields.

**Data record**

The data were organized according to the Brain-Imaging-Data-Structure (BIDS) Specification version 1.0.2 and can be accessed from the OpenNeuro public repository (accession number: XXX). In short, raw data of each subject were stored in “sub-<ID>” directories; The pre-processed volume data and the  surface-based data can be found in “derivatives/pre-processing” and “derivatives/volumetosurface” directories, respectively.

*Stimulus*
The stimulus for different fMRI experiments are stored as “stimuli”. 

*Raw MRI data*
Each participant's folder is comprised of 2 session folders: “sub-<subID>/ses-anat” ,“sub-<subID>/ses-01”.The “ses-anat” folder comprises one folders, named “anat”.The “ses-01” folder comprises two folders, named“func” or “fmap”.A “sub-<subID>/sub-<subID>_ses-01_scans.tsv” file stores the scan information for a scan session. The task events were saved as“sub-<subID>/func/sub-<subID>_ses-01_task-<taskID>_run-<runID>_events.tsv”for each run.

*Freesurfer recon-all*
The results of reconstructing the Cortical Surface were saved as “derivatives/recon-all-FreeSurfer/sub-<subID>” folders.

*Pre-processed volume data from pre-processing*
The pre-processed volume-based fMRI data were saved as“pre-processed_volume_data/sub-<subID>/ses-01/sub-<subID>_ses-01_task-<taskID>_volume_run-<runID>.nii”.

*Preprocessed surface-based data*
The pre-processed surface-based data were saved as “derivatives/volumetosurface/sub-<subID>/task-<taskID>_run-<index>_lh/rh.surfacedata.mat” for each run.

*The technical validation of the NFED*
The results of the technical validation were saved as “derivatives/validation/results” for each participant.The code of the technical validation were saved as “derivatives/validation/code”.
