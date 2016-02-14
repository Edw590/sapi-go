tts - A lightweight python TTS wrapper
======================================
tts is a python wrapper around Text To Speech api's

Currently only supports SAPI

Setup
-----
To install, simply use pip and point it at the repository

```
pip install git+https://github.com/DeepHorizons/tts
```

To Use
------
Import the tts package with the api you wish to use

### SAPI
```python
import tts.sapi
voice = tts.sapi.Sapi()
voice.say("Hello")
voice.set_voice("Anna")
voice.create_recording('output.wav', "This will be in a wav file")
voice.rate(-5)
voice.say("This will be said slower")
```

The SpVoice COM object is available as the voice variable in the instance of the Sapi class.
https://msdn.microsoft.com/en-us/library/ee125640%28v=vs.85%29.aspx
Properties are assigned and read from, Methods are used like functions.

Happy Hacking