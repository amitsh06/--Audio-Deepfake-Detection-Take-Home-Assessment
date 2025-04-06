# Audio Deepfake Detection Project

## Overview
This project implements audio deepfake detection techniques based on research from the [Audio-Deepfake-Detection](https://github.com/media-sec-lab/Audio-Deepfake-Detection) repository. The implementation includes research on promising approaches, selection of a model for implementation, and documentation of the process.

## Project Structure
```
├── README.md                 # Project overview and instructions
├── requirements.txt          # Dependencies for the project
├── notebooks/                # Jupyter notebooks for implementation
│   ├── model_implementation.ipynb  # Main implementation notebook
├── research/                 # Research documentation
│   ├── approach_analysis.md  # Analysis of selected approaches
├── data/                     # Directory for datasets (to be downloaded)
└── docs/                     # Additional documentation
    └── final_report.md       # Final analysis and documentation
```

## Setup Instructions

1. Clone the repository:
   ```
   git clone https://github.com/your-username/audio-deepfake-detection.git
   cd audio-deepfake-detection
   ```

2. Create and activate a virtual environment:
   ```
   python -m venv venv
   # On Windows
   venv\Scripts\activate
   # On macOS/Linux
   source venv/bin/activate
   ```

3. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

4. Download the dataset:
   - The notebook contains instructions for creating a demo dataset
   - For full implementation, download the ASVspoof 2019 dataset from [the official website](https://www.asvspoof.org/index2019.html)

## Usage

1. Open the Jupyter notebook:
   ```
   jupyter notebook notebooks/model_implementation.ipynb
   ```

2. Follow the implementation steps in the notebook to:
   - Prepare the dataset
   - Extract audio features
   - Train the LCNN with Attention model
   - Evaluate the model performance

## Model Architecture

The implementation uses a Light Convolutional Neural Network (LCNN) with Attention Mechanism, selected for its excellent balance between performance and computational efficiency. The attention mechanism is particularly well-suited for detecting the subtle artifacts present in deepfake audio.

## Results

The model achieves competitive performance on audio deepfake detection tasks, with detailed analysis available in the final report document.

## License

This project is available for educational and research purposes.

## Acknowledgements

This implementation is based on research from the [Audio-Deepfake-Detection](https://github.com/media-sec-lab/Audio-Deepfake-Detection) repository.