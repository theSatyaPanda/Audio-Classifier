#### Dataset-
I used UrbanSound8K dataset because it was the largest dataset I could found. It include 8,732 WAV files all less or equal to 4 seconds in duration across 10 different classes:
  - air_conditioner
  - car_horn
  - children_playing
  - dog_bark
  - drilling
  - enginge_idling
  - gun_shot
  - jackhammer
  - siren
  - street_music
#### Library- 
Here I used Librosa library which is popularly used for Audio Signal Processing because it helps to converge signals into monochannel, it can represent a audio signal in a normalize pattern (i.e between -1 to +1), so that a regular pattern is observed from all the audio signals and it can vizualize the sample rate.
#### Extract Features-
Here I used Mel-Frequency Cepstral Cofficients(MFCC) from audio samples. MFCC summarises the frequency distribution across window size, so it is possible to analyse both frequency and time characteristics of the sound.These audio representations will allow us to identify features for classification.
#### Model Creation- 
I used Tensorflow 2.2.0. To check accuracy I used library like Sequential, Dense, Dropout, Activation and Flatten. The test accuracy after 100 epochs and a batch size of 32 is 80.14 %.
#### Testing audio data-
###### Steps I followed
Preprocessed the new audio data
Predicted the classes
Inverse transform my predicted level
