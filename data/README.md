# Dataset Directory

This directory is intended for storing the audio datasets used in the deepfake detection project.

## Recommended Datasets

### ASVspoof Dataset

The ASVspoof dataset is recommended for this implementation. It contains both genuine and spoofed audio samples designed to help develop countermeasures against spoofing attacks on automatic speaker verification (ASV) systems.

### Download Instructions

The ASVspoof dataset can be downloaded from the official website:
- [ASVspoof 2019](https://www.asvspoof.org/index2019.html)
- [ASVspoof 2021](https://www.asvspoof.org/index2021.html)

After downloading, extract the dataset into this directory maintaining the following structure:

```
data/
├── ASVspoof2019/
│   ├── LA/
│   │   ├── ASVspoof2019_LA_train/
│   │   ├── ASVspoof2019_LA_dev/
│   │   └── ASVspoof2019_LA_eval/
│   └── protocols/
└── README.md
```

## Alternative Datasets

Other datasets that can be used for audio deepfake detection include:

1. **FakeAVCeleb**: A dataset containing both fake audio and video
2. **WaveFake**: A dataset specifically for audio deepfake detection
3. **In-the-Wild Dataset**: Real-world examples of deepfake audio

More datasets can be found in the [Audio-Deepfake-Detection repository](https://github.com/media-sec-lab/Audio-Deepfake-Detection?tab=readme-ov-file#datasets).

## Data Preprocessing

The implementation notebook contains code for preprocessing the audio data, including:
- Loading audio files
- Extracting MFCC features
- Normalizing features
- Preparing data for model training

Refer to the `notebooks/model_implementation.ipynb` file for detailed preprocessing steps.