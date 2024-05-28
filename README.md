# dataset_LongitudinalNoTreatement

## Participants:

For this study 27 participants with chronic lower back pain (14 males, 13 females) and 25 control participants (10 males, 15 females) were recruited and scanned at 3 time points (0, 2 and 4 months) in Sherbrooke, Quebec, Canada (april 2021 to july 2022). Inclusion/exclusion protocol made sure that participants were over 18 years old, had pain primarily localized in the lower back for more than 16 weeks (4 months) prior to first visit with or without pain radiating to the legs or radiating to the neck, had a pain visual analogue scale score (VAS) over 30 mm within the last 24 hours (maximum of 100 mm), had no history of neurological or psychiatric impairment and did not use medication such as: cortisone infiltrations (within last 2 years), chronic opioids and antidepressants. 


## MRI data:

All participants were imaged using a 3.0 T MRI scanner (Philips Ingenia, Siemens) across T1-weighted, BOLD, TOF, SWI and diffusion weighted contrasts. 

T1-weighted images (~ 5 min) were obtained using a MAG prepared (MP) Gradient Recalled (GR) sequence with repetition time (RT) = 7.9 ms, echo time (TE) = 3.5 ms, flip angle = 8°, voxel size 1.00mm x 1.00mm x 1.00mm. 

BOLD images (~ 10 min) were obtained using a 2D segmented k-space (SK) Fat Saturation (FS) Gradient recalled (GR) sequence with repetition time (RT) = 1.075 s, echo time (TE) = 30 ms, flip angle = 55°, voxel size 3.00mm x 3.00mm x 3.00mm. For each subject 576 volumes were obtained including 1 reversed phase encoding (AP) volume for correcting susceptibility induced distortions. SENSE = 1.2 and multi band (MB) = 4

Diffusion-weighted images (~ 9 min) were obtained using a 2D segmented k-space (SK) Fat Saturation (FS) Spin Echo (SE) sequence with repetition time (RT) = 4.800 s, echo time (TE) = 92 ms, flip angle = 90°, voxel size 2.00mm x 2.00mm x 2.00mm. For each subject 108 diffusion volumes (7 b = 0 mm2/s, 8 b = 300 mm2/s, 32 b = 1,000 mm2/s, 60 b = 2,000 mm2/s) were obtained including a b0 with reverse phase encoding (AP) for correction of susceptibility induced distortions. SENSE = 1.9

...


## Notes on data:
see the excel file for easy visualization of valid acquisition per visit and imaging modalities

### decouverte fortuite (rejected subjects in dataset_outlier)
#subject sub-018 was removed (decouverte fortuite at first visit v1)

### absent visits
subjects sub-037, sub-039, sub-008 have only first visit v1
subject sub-016 has only first and second visit (v1 and v2)
subject sub-019_v3 missing QSM

subjects sub-007_ses-v3, sub-010_ses-v2 had problems during acquisition and a .5 version is available (use that)
subject sub-012_ses-v2 DWI resolution: 1.76mm x 1.76mm x 2.00mm, the DWI image was kept (normal reverse acq, good TOPUP results on visual inspection, brainstem slightly cut)
subject sub-014_ses-v3 DWI resolution: 2.00mm x 2.00mm x 2.24mm, the DWI image was kept (normal reverse acq, good TOPUP results on visual inspection)
subject sub-019_ses-v3 T1w resolution: 0.99mm x 0.99mm x 1.00mm, the T1w image was kept
subject sub-031_ses-v1 T1w resolution: 0.96mm x 0.96mm x 1.00mm, the T1w image was kept

### weird acquisiton removed (rejected acquistion in dataset_outlier)
subject sub-004_ses-v2 BOLD resolution: 3.00mm x 3.00mm x 3.00mm x 2.07s, the BOLD image was removed (normal reverse acq)
subject sub-035_ses-v1 BOLD resolution: 3.00mm x 3.00mm x 3.00mm x 2.07s, the BOLD image was removed (normal reverse acq)
subject sub-057_ses-v2 BOLD was removed (lost reverse acq for fmri)
subject sub-004_ses-v1 BOLD and DWI was removed (lost reverse acq for fmri + dmri)

### mutliple runs (rejected runs in dataset_outlier)
subject sub-014_ses-v1 DWI was taken twice because first image has movement, run 2 was kept
subject sub-019_ses-v1 DWI was taken twice because first image was to blurry, run 2 was kept
subject sub-025_ses-v1 DWI was taken twice because first image has movement, run 2 was kept
subject sub-034_ses-v2 QSM was taken twice (no mention in redcap but more artifacts visible on run 1), run 2 was kept
subject sub-035_ses-v2 QSM was taken twice (no mention in redcap but more artifacts visible on run 1), run 2 was kept


## Slice timing for fMRI:

0	2	4	11	9	7	1	3	5	10	8	6
12	14	16	23	21	19	13	15	17	22	20	18
24	26	28	35	33	31	25	27	29	34	32	30
36	38	40	47	45	43	37	39	41	46	44	42

0, 12, 24 and 36 were acquired in parallel at t=0
2, 14, 26 and 38 were acquired in parallel at t=TR/12
...




