# Image Captioning Using Attention Networks - 670 Project

## To Train

This was written in python3 so may not work for python2. Download the COCO dataset training and validation
images. Put them in `data/coco/imgs/train2014` and `data/coco/imgs/val2014` respectively. Put the COCO
dataset split JSON file from [Deep Visual-Semantic Alignments](https://cs.stanford.edu/people/karpathy/deepimagesent/)
in `data/coco/`. It should be named `dataset.json`.

Run the preprocessing to create the needed JSON files:

```bash
python generate_json_data.py
```

Start the training by running:

```bash
python train.py
```

## To Generate Captions

```bash
python generate_caption.py --img-path <PATH_TO_IMG> --model <PATH_TO_MODEL_PARAMETERS>
```
