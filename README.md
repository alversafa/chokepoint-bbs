# ChokePoint Dataset Bounding Box Annotations

Bounding box annotations for the G1 and G2 sets of the ChokePoint dataset, provided
as a supplementary material to:

S. Alver and U. Halici, **"Attentive Deep Regression Networks for Real-Time Visual 
Face Tracking in Video Surveillance,"** Submitted, 2019.

## Description

This repository contains bounding box annotations for the G1 and G2 sets (sets for
the baseline verification protocol) of the
[ChokePoint dataset](http://arma.sourceforge.net/chokepoint/). For the ease of 
training (or development) and evaluation, we provide two folders: `G1` and `G2`.
These folders have a `train_annotation.txt` file that contains the training annotations
for that folder. They also have 216 separate `eval_annotation_seq_X.txt` files that
contain the evaluation annotations for the 216 different sequences in the evaluation
set. We provide them separately so that the performance on each of the evaluation
sequences can be examined individually. Each of the lines in these files are in the
form of: `file_directory+file_name, top_left_row, top_left_column, width, height`. 

**NOTE:** The original dataset only has person ID and eye location annotations, 
which makes it incompatible with the task of visual face tracking.


## Citation

If you find this work to be useful for your studies, please cite (using the BibTeX
entries) the following two articles:

```
@misc{alver_2019,
  Author = {Safa Alver and Ugur Halici},
  Title = {Attentive Deep Regression Networks for Real-Time Visual Face Tracking
  in Video Surveillance},
  Year = {2019},
  Eprint = {arXiv:1908.03812},
}
```

```
@inproceedings{wong_cvprw_2011,
   Author = {Yongkang Wong and Shaokang Chen and Sandra Mau and Conrad Sanderson
   and Brian C. Lovell},
   Title = {Patch-based Probabilistic Image Quality Assessment for Face Selection
   and Improved Video-based Face Recognition},
   Booktitle = {IEEE Biometrics Workshop, Computer Vision and Pattern Recognition
   (CVPR) Workshops},
   Year = {2011},
   Pages = {81-88},
   Month = {June},
   Publisher = {IEEE}
}
```
