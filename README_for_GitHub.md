# Audio Deepfake Detection Project

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Overview
This project implements audio deepfake detection techniques based on research from the [Audio-Deepfake-Detection](https://github.com/media-sec-lab/Audio-Deepfake-Detection) repository. The implementation includes research on promising approaches, selection of a model for implementation, and documentation of the process.

The project uses a Light Convolutional Neural Network (LCNN) with Attention Mechanism, selected for its excellent balance between performance and computational efficiency. The attention mechanism is particularly well-suited for detecting the subtle artifacts present in deepfake audio.

## Project Structure
```
├── README.md                 # Project overview and instructions
├── requirements.txt          # Dependencies for the project
├── notebooks/                # Jupyter notebooks for implementation
│   ├── model_implementation.ipynb  # Main implementation notebook
├── research/                 # Research documentation
│   ├── approach_analysis.md  # Analysis of selected approaches
├── data/                     # Directory for datasets (to be downloaded)
├── docs/                     # Additional documentation
│   └── final_report.md       # Final analysis and documentation
└── images/                   # Visualizations and diagrams
    ├── accuracy_curve.png    # Model accuracy visualization
    └── loss_curve.png        # Model loss visualization
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

4. Dataset Setup:
   This project uses the [ASVspoof 2019 LA](https://datashare.ed.ac.uk/handle/10283/3336) dataset.
   - Download the dataset from the official source
   - Extract the audio files into the `data/` folder
   - The dataset contains bonafide and spoof audio samples for training and evaluation

## Implementation Details

This project follows a three-part approach:

1. **Research & Selection**: Analysis of three promising audio deepfake detection approaches
2. **Implementation**: Implementation of one selected approach with dataset integration
3. **Documentation & Analysis**: Comprehensive documentation of the process, challenges, and results

Detailed implementation and analysis can be found in the respective notebooks and documentation files.

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

The implementation uses a Light Convolutional Neural Network (LCNN) with Attention Mechanism. The attention mechanism helps the model focus on the most relevant parts of the audio signal for detecting deepfakes.

Key components:
- Spectral feature extraction
- Light CNN layers for efficient processing
- Attention mechanism to focus on artifacts
- Classification head for binary detection

## Results

The model achieves competitive performance on audio deepfake detection tasks, with detailed analysis available in the final report document.

## Contributing

Contributions are welcome! Please see the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

This implementation is based on research from the [Audio-Deepfake-Detection](https://github.com/media-sec-lab/Audio-Deepfake-Detection) repository.