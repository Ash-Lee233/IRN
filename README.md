# IRN

[Invertible Image Rescaling](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123460120.pdf)

Implementation of High-resolution digital images are usually downscaled to fit various
display screens or save the cost of storage and bandwidth, meanwhile the postupscaling is adpoted to recover the original resolutions or the details in the zoomin images.

# Dataset

[DIV2K](https://data.vision.ee.ethz.ch/cvl/DIV2K/)

# Train

```bash
bash run_standalone_train.sh [SCALE] [DATASET_GT_PATH]
# example: bash run_standalone_train.sh 4 /home/nonroot/IRN/data/DIV2K_train_HR
```

# Eval

```bash
bash run_eval.sh 4 /home/nonroot/IRN/data/DIV2K_valid_HR /home/nonroot/IRN/ckpt/latest.ckpt
```