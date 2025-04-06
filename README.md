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

1. Clone this repository
2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Dataset Setup:
   This project uses the [ASVspoof 2019 LA](https://datashare.ed.ac.uk/handle/10283/3336) dataset.
   - Download the dataset from the official source
   - Extract the audio files into the `data/` folder
   - The dataset contains bonafide and spoof audio samples for training and evaluation
4. Run the Jupyter notebooks in the `notebooks/` directory

## Implementation Details

This project follows a three-part approach:

1. **Research & Selection**: Analysis of three promising audio deepfake detection approaches
2. **Implementation**: Implementation of one selected approach with dataset integration
3. **Documentation & Analysis**: Comprehensive documentation of the process, challenges, and results

Detailed implementation and analysis can be found in the respective notebooks and documentation files.

## Model Architecture

The implementation uses a Light Convolutional Neural Network (LCNN) with Attention Mechanism, selected for its excellent balance between performance and computational efficiency. The attention mechanism is particularly well-suited for detecting the subtle artifacts present in deepfake audio.

## Results

The model achieves competitive performance on audio deepfake detection tasks, with detailed analysis available in the final report document.

## License

This project is available for educational and research purposes.

## Acknowledgements

This implementation is based on research from the [Audio-Deepfake-Detection](https://github.com/media-sec-lab/Audio-Deepfake-Detection) repository.