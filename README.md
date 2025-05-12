# REALTIME_STT-NM
Unit 5 This Jupyter Notebook performs audio signal processing to extract features such as MFCC, pitch, energy, and SNR from a dataset of audio files. It then classifies audio files as either clean or noisy based on a Signal-to-Noise Ratio (SNR) threshold and exports the results as a CSV file for further analysis, such as visualization in Power BI.

📁 Dataset The audio files are located in a specified directory (dev-clean) on your system.

Supported audio formats: .wav, .mp3, .flac, .ogg

🔍 Features Extracted MFCC (Mel Frequency Cepstral Coefficients)

Pitch (using YIN algorithm)

Energy

SNR (Signal-to-Noise Ratio)

Duration

🧪 Processing Steps Walk through all audio files in the given directory.

Load each file at 16kHz sample rate using librosa.

Extract features mentioned above.

Estimate SNR and label the file:

If SNR > 10 dB → label as "clean"

Else → label as "noisy"

Save the extracted metadata and features to a CSV file: audio_features_metadata_5.csv.

📦 Requirements Python

librosa

numpy

pandas

soundfile

tqdm

Install using:

pip install librosa pandas numpy soundfile tqdm 📝 Output audio_features_metadata_5.csv: Contains all extracted features and labels for use in visualization tools like Power BI.

