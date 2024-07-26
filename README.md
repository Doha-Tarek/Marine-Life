# Marine Life Analysis and Detection

## Project Overview

This project focuses on analyzing and enhancing underwater videos to classify and detect underwater animals and objects. The project involves building transfer learning models and implementing various image enhancement techniques to improve the clarity and accuracy of the analysis.

### Key Components

1. **Transfer Learning Models**: Built using VGG16, DenseNet, and ResNet50 architectures to classify underwater animals and objects.
2. **Object Detection and Instance Segmentation**: Implemented using YOLOv8 to detect and segment underwater animals.
3. **Image Enhancement**: Applied Gray-World Algorithm, Histogram Equalization, and CLAHE for enhancing video quality.
4. **Edge Detection**: Utilized Canny Edge Detector for edge detection in underwater images.

## Installation Instructions

1. Clone the repository:

    ```sh
    git clone https://github.com/Doha-Tarek/Marine-Life.git
    cd Marine-Life
    ```

2. Set up a virtual environment:

    ```sh
    python3 -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```


## Usage Instructions

1. Run the Jupyter notebooks to see the implementation and results.
2. Modify the notebooks as needed for your specific use case.
3. Use the provided scripts to train and evaluate models on your own datasets.

## Results

The models have been trained and evaluated on a dataset of underwater videos, achieving high accuracy in classifying and detecting underwater animals and objects. Detailed results and metrics are available in the respective notebooks.


