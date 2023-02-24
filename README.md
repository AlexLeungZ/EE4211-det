# object-detector

Object Detector using HOG as descriptor and Linear SVM as classifier.

## Configuration File

```bash
[hog]
min_wdw_sz: [100, 40]
step_size: [10, 10]
orientations: 9
pixels_per_cell: [8, 8]
cells_per_block: [3, 3]
visualize: False
normalize: True

[nms]
threshold: .3
```

## About the modules

* `extract-features.py` -- This module is used to extract HOG features of the training images.
* `train-classifier.py` -- This module is used to train the classifier.
* `nms.py` -- This module performs Non Maxima Suppression.
* `test-classifier.py` -- This module is used to test the classifier using a test image.
* `config.py` -- Imports the configuration variables from `config.cfg`.
