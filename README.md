# Image Quality Assessment Tools

This repository contains tools for evaluating image quality using various perceptual metrics, including PSNR, SSIM, and LPIPS.

## Overview

This toolkit provides implementations of several image quality assessment metrics and utilities for comparing distorted images against their reference versions. It's particularly useful for researchers and developers working in image processing, computer vision, and deep learning.

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/image-quality-assessment.git
cd image-quality-assessment

# Install required packages
pip install -r requirements.txt
```

## Requirements

- Python 3.7+
- lpips
- scikit-image
- numpy
- pandas
- scipy
- matplotlib
- PIL
- torch

## Usage

```python
from quality_metrics import calculate_psnr, calculate_ssim, calculate_lpips

# Load your images
img1 = load_image("path/to/reference.png")
img2 = load_image("path/to/distorted.png")

# Calculate metrics
psnr_score = calculate_psnr(img1, img2)
ssim_score = calculate_ssim(img1, img2)
lpips_score = calculate_lpips_vgg(img1, img2)
```

## Features

- Multiple image quality metrics:
  - Peak Signal-to-Noise Ratio (PSNR)
  - Structural Similarity Index (SSIM)
  - Learned Perceptual Image Patch Similarity (LPIPS)
    - VGG-based implementation
    - AlexNet-based implementation
- Batch processing capabilities
- Data analysis utilities
- Correlation analysis with human perception scores

## Directory Structure

```
.
├── src/
│   ├── metrics/
│   │   ├── psnr.py
│   │   ├── ssim.py
│   │   └── lpips.py
│   ├── utils/
│   │   ├── image_processing.py
│   │   └── data_analysis.py
├── tests/
├── examples/
├── requirements.txt
└── README.md
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Citation

If you use this code in your research, please cite:

```bibtex
@misc{image-quality-assessment,
  author = {Your Name},
  title = {Image Quality Assessment Tools},
  year = {2024},
  publisher = {GitHub},
  url = {https://github.com/yourusername/image-quality-assessment}
}
```
