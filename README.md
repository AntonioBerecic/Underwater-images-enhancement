# Underwater-images-enhancement

This project aims to enhance underwater images using classic image processing and computer vision techniques. Underwater photographs are often degraded by light absorption and scattering, resulting in poor contrast, color distortion, and blurred details. This repository provides a step-by-step workflow for improving the visual quality of such images.

## Features

- **Dehazing:** Removes haze caused by light scattering in water using the Dark Channel Prior algorithm.
- **White Balance:** Corrects color shifts by stretching the histogram of each RGB channel.
- **Color Correction:** Adjusts the color balance, with emphasis on restoring the red channel typically lost underwater.
- **Contrast Enhancement:** Uses Contrast Limited Adaptive Histogram Equalization (CLAHE) to boost local contrast.
- **Sharpening:** Employs Unsharp Masking to highlight fine details and edges.

## Technologies Used

- Python (Jupyter Notebook)
- OpenCV (`cv2`)
- NumPy
- Matplotlib
- scikit-image (for quantitative evaluation metrics such as PSNR and SSIM)

## Dataset

- A subset of the [UIEB Underwater Image Enhancement Benchmark](https://li-chongyi.github.io/Proj_Underwater/), consisting of pairs of raw and reference images for qualitative and quantitative evaluation.

## Usage

1. Clone this repository: git clone https://github.com/AntonioBerecic/Underwater-images-enhancement
2. Install the dependencies (preferably in a virtual environment): pip install opencv-python numpy matplotlib scikit-image
3. Open the provided Jupyter Notebook and follow the workflow to process images.
4. Test images: Place your underwater images in the `/images` directory and update the notebook paths as needed.

## Results

- Evaluation includes both visual comparisons and quantitative metrics (PSNR, SSIM), demonstrating substantial improvements in contrast and color balance. Some limitations and artifacts (e.g., halos, over-correction) may occur, especially with extreme or unbalanced inputs.

## Limitations

- The processing pipeline is tuned for typical underwater conditions and may need adjustments for specific cameras or environments.
- Fixed parameters may not suit all images or lighting situations and could introduce artifacts on some datasets.

## Author

Antonio Berečić

## References
- C. Li, C. Guo, W. Ren, R. Cong, J. Hou, S. Kwong, D. Tao, An underwater imageenhancement benchmark dataset and a benchmark. IEEE Trans. Image Process. 2019, 29, 4984-5001.
- [Project paper: POBOLJSANJE PODVODNIH FOTOGRAFIJA](POBOLJSANJE_PODVODNIH_FOTOGRAFIJA.pdf)
