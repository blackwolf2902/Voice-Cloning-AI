# Voice Cloning AI

This repository contains code that demonstrates voice cloning using the Tortoise-TTS library in a Google Colab notebook.

Note: This project was created specifically for the AI Engineer Intern task at OpeninApp Company. The Voice Cloning AI showcases the ability to synthesize speech with custom voice data using HuggingFace models. The provided sample input and output audio files demonstrate the successful completion of the task.

Feel free to connect with me on LinkedIn: [www.linkedin.com/in/arumugam-n-436466238]

## Getting Started

1. Install Dependencies:
   Make sure you have the necessary libraries installed by running the following commands in the Colab notebook:
   ```python
   !pip3 install -U scipy
   !pip3 install -r requirements.txt
   !pip3 install transformers==4.19.0 einops==0.5.0 rotary_embedding_torch==0.1.5 unidecode==1.3.5
   !python3 setup.py install
   ```

2. Load Libraries and Models:
   The notebook loads the required libraries and models, including the HuggingFace models used by Tortoise.

3. Custom Voice Upload:
   In this code, you can upload at least two audio clips (in WAV format) of the same speaker, each 6-10 seconds long. This custom voice is used to generate synthesized speech with the target speaker's voice characteristics.

4. Generate Speech:
   The notebook generates speech with the custom voice using the provided text and preset mode. Change the `text` variable to use different text for synthesis. The `preset` variable determines the quality mode ("ultra_fast," "fast," "standard," or "high_quality").

5. Audio Output:
   The synthesized speech is saved as a WAV file named "generated-CUSTOM_VOICE_NAME.wav" (assuming the custom voice name is "CUSTOM_VOICE_NAME") in the current directory. The synthesized speech is also played using IPython display for audio output.

## Results

### Input:
Text: "Thanks for reading this article. I hope you learned something."

### Output:
https://github.com/blackwolf2902/Voice-Cloning-AI/blob/main/generated-joe.wav

Note: The quality of synthesized speech heavily depends on the amount and quality of custom voice data provided. The provided sample output is for demonstration purposes only and may not represent optimal results. The audio output can be further improved by using high-quality custom voice data and experimenting with different text inputs.

## Usage

1. Upload Custom Voice: 
   - Prepare at least two audio clips of the same speaker (6-10 seconds long) in WAV format.
   - Change the `CUSTOM_VOICE_NAME` variable to your desired custom voice name.
   - Upload the audio clips to Google Colab.

2. Generate Speech:
   - Modify the `text` variable to use your desired text for speech synthesis.
   - Adjust the `preset` variable to select the quality mode.

3. Execute the Code:
   - Run the cells in the Colab notebook to install dependencies and load models.
   - Upload the custom voice audio clips as instructed.
   - The synthesized speech with the custom voice will be generated and saved as "generated-CUSTOM_VOICE_NAME.wav" in the current directory.
   - The synthesized speech will also be played using IPython display.

## Note
- This code utilizes the Tortoise-TTS library, which is built on top of HuggingFace models, making it easy to experiment with voice cloning tasks.
- Be aware of the legal and ethical implications when using voice cloning technology, ensuring you have the necessary consent for using the custom voice data.

Enjoy experimenting with voice cloning using the Tortoise-TTS library!
