# SAR Image Colorization and Analysis

This project focuses on the colorization and analysis of Synthetic Aperture Radar (SAR) images using GAN-based architectures. The objective is to enhance SAR images by colorizing them in Near-Infrared (NIR) and Short-Wave Infrared (SWIR) ranges and subsequently applying object detection and classification models to extract relevant information.

## Project Goals

- **Colorization of SAR Images**: Using GAN (Unet + PatchGAN) to generate colorized SAR images for enhanced visual representation.
- **Object Detection and Classification**: Utilizing models such as YOLOv8 and ResNet-50 to perform object detection and classification on colorized SAR images.
- **Data Analysis**: Evaluate the performance of colorization and classification for different land covers, including agriculture, barren land, grassland, and urban.

## Table of Contents

- [Installation](#installation)
- [Dataset Structure](#dataset-structure)
- [Usage](#usage)
- [Model Configuration](#model-configuration)
- [Visualizations](#visualizations)
- [Future Work](#future-work)
- [License](#license)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/sar-image-colorization.git
   cd sar-image-colorization

## Dataset Structure
Organize your dataset with the following directory structure:

data/
├── agriculture/
│   ├── s1/  # Contains Sentinel-1 SAR images
│   └── s2/  # Contains Sentinel-2 images
├── barren/
│   ├── s1/
│   └── s2/
├── grassland/
│   ├── s1/
│   └── s2/
└── urban/
    ├── s1/
    └── s2/

Each folder should contain subdirectories for Sentinel-1 (SAR images) and Sentinel-2 images.

## Usage
Training GAN for Colorization:

Run the GAN training script to colorize SAR images.
Use the main_code/main.ipynb notebook to start the colorization process and monitor the training progress.
Object Detection and Classification:

After colorizing images, use YOLOv8 and ResNet-50 for object detection and classification.
Adjust the model configurations as needed in the script folder.
Evaluation:

Compare model accuracy for each land cover type (e.g., agriculture, barren land).
Generate visualizations to evaluate the colorization and classification results.

## Model Configuration
GAN Model: Modify the Unet + PatchGAN parameters in main_code/main.ipynb.

## Visualizations 
- Colorized results can be visualized directly from the output images in the results/ directory.
- Generate comparison plots to evaluate colorization effectiveness and classification accuracy using tools like Matplotlib.

## Future Work
Implement colorization in additional spectral bands.
Improve object detection accuracy with more advanced models.
Automate data preparation and augmentation processes for larger datasets.

## License
This project is licensed under the MIT License. See the LICENSE file for more information.


This README provides a detailed overview and setup instructions for your SAR project, including colorization and classification tasks. Let me know if you'd like to add anything further!


