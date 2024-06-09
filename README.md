# Urban_sound_classification

## Description

This project revolves around a dataset containing 8732 labeled sound excerpts (<=4s) of urban sounds from 10 distinct classes:

- Air Conditioner
- Car Horn
- Children Playing
- Dog Bark
- Drilling
- Engine Idling
- Gun Shot
- Jackhammer
- Siren
- Street Music

The classes are based on the urban sound taxonomy described in the following article:

*J. Salamon, C. Jacoby and J. P. Bello, "A Dataset and Taxonomy for Urban Sound Research", 22nd ACM International Conference on Multimedia, Orlando USA, Nov. 2014.*

The dataset comprises audio excerpts sourced from field recordings uploaded to [Freesound](https://freesound.org/). To facilitate reproducibility and comparison of automatic classification results, the files are pre-sorted into ten folds (folders named fold1-fold10).

Additionally, a CSV file named `UrbanSound8k.csv` is provided, containing metadata about each audio excerpt.

## Included Files

### Audio Files

- **8732 audio files** of urban sounds in WAV format.

### Meta-data Files

- **UrbanSound8k.csv**: Contains metadata information about every audio file in the dataset. Each entry includes:

  - `slice_file_name`: Name of the audio file.
  - `fsID`: Freesound ID of the recording.
  - `start`: Start time of the slice in the original recording.
  - `end`: End time of the slice in the original recording.
  - `salience`: Subjective salience rating of the sound (1 = foreground, 2 = background).
  - `fold`: Fold number (1-10) to which the file is allocated.
  - `classID`: Numeric identifier of the sound class.
  - `class`: Class name.

## Usage

1. Clone this repository:

git clone https://github.com/shreyash18g/Urban_sound_classification.git


## Data Exploration

### Metadata Analysis

The dataset includes a CSV file named `UrbanSound8k.csv` containing metadata about each audio excerpt. You can perform metadata analysis to understand the distribution of classes, the duration of sound clips, and other relevant information.

## Visualize Audio Waveforms and Spectrograms

Visualizing audio waveforms and spectrograms can provide insights into the characteristics of different urban sounds. You can use libraries such as matplotlib and librosa to plot waveforms and spectrograms.

## Feature Extraction

Feature extraction is a crucial step in preparing data for model training. Common features used for audio classification include Mel-Frequency Cepstral Coefficients (MFCCs), Spectral Centroid, and Zero Crossing Rate. Extracting these features will help in building a robust classification model.

## Model Training

### Develop and Train Classification Models

You can develop classification models using popular deep learning frameworks such as TensorFlow or PyTorch. Architectures like Convolutional Neural Networks (CNNs) and Recurrent Neural Networks (RNNs) are commonly used for audio classification tasks. Experiment with different architectures and hyperparameters to find the best model for your dataset.

## Evaluate Model Performance

Once the models are trained, evaluate their performance using appropriate metrics such as accuracy, precision, recall, and F1-score. Additionally, consider using techniques like cross-validation to ensure the reliability of your results.

## Contributing

Contributions to this project are welcome! Whether you want to suggest improvements, report issues, or contribute code, feel free to submit pull requests or open issues on the project's GitHub repository.




