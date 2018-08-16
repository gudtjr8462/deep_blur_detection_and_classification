# deep_blur_detection_and_classification

Tensorflow implementation of "Defocus and Motion Blur Detection with Deep Contextual Features"

For image examples:

![input2](./input/out_of_focus0607.jpg) ![output2](./output/out_of_focus0607.png)

This repository contains a test code and sythetic dataset, which consists of scenes including motion and defocus blurs together in each scene for reproduce.

--------------------------

## Prerequisites
- Ubuntu 16.04
- Tensorflow 1.6.0 or higher
- Tensorlayer 1.8.2 or higher
- Opencv2

## Test Details
- download a model weights from [google drive](https://drive.google.com/open?id=1gaUmaZttnXB9Ya1JmM7jOsUeUeSPIvVj) and save the model into 'model' folder.
- specify a path of input folder in 'main.py' at line #39
- run 'main.py'

```bash
python main.py
```
## Synthetic Dataset
- download [synthetic train set](https://drive.google.com/open?id=1LPaHkuQXziBWqEsM4cIwzzkcLxbupID1)(337MB) and [synthetic test set](https://drive.google.com/open?id=1wEhXlvq1wHO05HjtbDXDqnGu2q-ZFEsQ)(11.5MB)
- Note that sharp pixels, defocus-blurred pixels, and motion-blurred pixels are labeled as 0, 100, and 200 in the [0,255] range.