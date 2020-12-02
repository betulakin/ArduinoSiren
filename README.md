# ArduinoSirenCall
 


There was a small piece of code they asked us to write on the job application. The script is this;

Using the Arduino based SD Card or its own memory (sound file, 10 separate alarm police, ambulance, fire brigade ...) if we send 1 data from the serial port, the alarm number 1 will sound, if 2 is sent, 2 ... 0 will be stopped if it is sent. Let the sound quality be at least 8 bits. PCM library can be used.

Using the Arduino's own memory, 10 kinds of alarms encoded, unfortunately, does not fit into the Arduino memory. Therefore, I recommend those who will use more than one siren sound to use Arduino Sd card module.

We need to do a few steps to get the siren sounds into our code. First, we convert it to 16-PCM format in an audio file editing program and make the necessary selection to make it 8-bit. After exporting, we encode the audio file with the encode program and get the values. You can define the values you received as a global variable on Arduino IDE and paste the values into the array.
