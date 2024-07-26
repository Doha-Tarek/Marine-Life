# Marine Life Analysis and Detection

## Project Overview

This project aims to leverage advanced machine learning techniques to analyze and enhance underwater videos, enabling the accurate classification and detection of underwater animals and objects. The project encompasses several key components, including transfer learning models, object detection and instance segmentation, image enhancement, and edge detection. Each component plays a vital role in improving the clarity and accuracy of the analysis.

### Key Components

1. **Image Enhancement**:
    - Underwater images often suffer from poor visibility and color distortion due to the scattering and absorption of light. To address these issues, we applied several image enhancement techniques:
        - **Gray-World Algorithm**: This algorithm adjusts the color balance of underwater images, compensating for the blue-green color cast typically observed in underwater environments.
        - **Histogram Equalization**: This technique enhances the contrast of images by uniformly distributing the intensity values, making the features more distinguishable.
        - **CLAHE (Contrast Limited Adaptive Histogram Equalization)**: An advanced form of histogram equalization that operates on small regions in the image, preventing over-amplification of noise while enhancing local contrast.

2. **Edge Detection**:
    - Edge detection is crucial for identifying the boundaries and shapes of objects within an image. We employed the **Canny Edge Detector**, a popular edge detection algorithm known for its effectiveness and precision.
    - The Canny Edge Detector works by identifying areas of rapid intensity change, highlighting the edges of underwater animals and objects.
    - This information is invaluable for further processing steps, such as segmentation and object recognition, ensuring that the edges are accurately detected and utilized.

3. **Transfer Learning Models**:
    - We utilized pre-trained models such as **VGG16**, **DenseNet**, and **ResNet50** to classify underwater animals and objects.
    - Transfer learning allows us to take advantage of these models' pre-existing knowledge, significantly reducing the amount of data and time required to train the models for our specific task.
    - Each model was fine-tuned on a dataset of underwater images to adapt to the unique characteristics of the underwater environment, such as varying lighting conditions and visibility.

4. **Object Detection and Instance Segmentation**:
    - For object detection and instance segmentation, we implemented **YOLOv8** (You Only Look Once version 8), a state-of-the-art deep learning model known for its speed and accuracy.
    - YOLOv8 was trained to detect and segment underwater animals in real-time, providing precise bounding boxes and segmentation masks for each detected object.
    - This enables the identification of multiple animals and objects within a single frame, facilitating detailed analysis of underwater scenes.

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
