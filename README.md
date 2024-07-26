# Simple Audio Transcriber
This transcription app uses OpenAI whisper in WatsonX to transcribe an uploaded audio file. Note: The length has been limited so if the audio file is long, it won't transcribe the whole thing.

First, you'll want to set up a virtual environment:

```
pip3 install virtualenv
virtualenv my_env # create a virtual environment my_env 
source my_env/bin/activate # activate my_env
```

Then you'll need to install the libraries you'll need, including Hugging Face Transformers, Gradio, Langchain, HuggingFaceHub and WatsonX LLM.

```
# installing required libraries in my_env
pip install transformers==4.35.2 torch==2.1.1 gradio==4.17.0 langchain==0.0.343 ibm_watson_machine_learning==1.0.335 huggingface-hub==0.19.4
```

Then install ffmpeg to be able to work with audio files in python:

```
sudo apt update
sudo apt install ffmpeg -y
```

To launch, type `python3 speech_analyzer.py` in the terminal.

This is running out of port 7860 so to access the app, you can visit http://127.0.0.1:7860/ or http://localhost:7860/ in your web browser.
