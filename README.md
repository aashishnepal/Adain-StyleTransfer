# Neural Style Transfer using AdaIN (Adaptive Instance Normalization)

This project implements Neural Style Transfer using Adaptive Instance Normalization (AdaIN) as described in the [Keras example](https://keras.io/examples/generative/adain/).

## Project Overview

This repository contains the implementation of a neural style transfer model that allows the blending of content and style images using AdaIN. The model is trained using a custom dataset, and progress can be tracked using a custom callback during the training process.

## Dataset

The dataset used for training this model is publicly available and can be downloaded from the following link:

- [Dataset Download Link](https://www.kaggle.com/datasets/ikarus777/best-artworks-of-all-time)

Please download the dataset and place it in the `data/` directory within the root of the project.

## Requirements

To run the project, ensure you have the following dependencies installed:

- TensorFlow
- Keras
- Matplotlib
- NumPy
- Python 3.x



## Usage

### Training the Model

To train the model, run the following command:

```bash
python train.py
```

### Monitoring Training Progress

Training progress is tracked using a custom callback that provides feedback on the percentage of completion for each epoch and the loss value. The training progress is printed to the console, and images are generated at the end of each epoch to visualize the content, style, and generated images.

### Speeding Up Training

To reduce training time, consider the following:
- Use a smaller subset of the dataset.
- Simplify the model architecture.
- Utilize mixed precision training if supported by your hardware.
- Ensure that the model is trained using a GPU or TPU.

### Customization

Feel free to modify the model architecture, dataset, or training parameters to suit your needs.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- The implementation is based on the [AdaIN Keras example](https://keras.io/examples/generative/adain/).
- Special thanks to the creators of the dataset and the Keras team for their valuable contributions.

