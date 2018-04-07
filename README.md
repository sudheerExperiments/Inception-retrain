# Image classification using Inception v3

This project uses Inception v3 pre-trained model to build a binary image classifier to classify classes goku and gohan. Inception v3 model is already trained with thousands of image classes, but not with images of goku and gohan (Dragon ball anime characters). The project retrains the classifier to detect two more new class images along with thousands of image classes trained before.

## Requirements:

Libraries: Python 3, Numpy, Scipy, Tensorflow.

## Usage:

Just make folder "data" with "goku" and "gohan" folders.

```
Inception-retrain/data
Inception-retrain/data/goku
Inception-retrain/data/gohan
```

## Train:

> python retrain.py --bottleneck_dir output_dir/bottleneck --summaries-dir output_dir/summaries --output_labels output_dir/output_labels.txt --model_dir inception/ --image_dir data/ --output_graph output_dir/output.pb --how_many_training_steps 500

## Test: 

> python retrain_model_classifier.py "data/gohan/images (4).png" 

## References:

1. [tensorflow_image_classifier](https://github.com/llSourcell/tensorflow_image_classifier)
2. [source dexter](https://sourcedexter.com/retrain-tensorflow-inception-model/)

