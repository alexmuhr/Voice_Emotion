# Voice Emotion
Detecting emotion in voices

### Business Case

Humans are very adept at detecting emotional cues in conversation and using these to inform concious
and unconcious decisions. The ability to detect emotion programatically holds enormous value. For example,
the ability to log emotion could be very helpful to customer service departments. Logs of customer emotion
could be used to tailor services, gauge customer satisfaction, or evaluate employee performance.

### Objective

Use the [RAVDESS](https://smartlaboratory.org/ravdess) and/or [TESS](https://tspace.library.utoronto.ca/handle/1807/24487)
datasets to train a classifier to infer emotion from auditory cues. In this application there is not a strong preference
for either precision or recall, so F1-score will be used as a key metric. Both the RAVDESS and TESS datasets classify
emotion into the categores anger, disgust, fear, happiness, pleasant surprise, sadness, and neutral.

### Scope and Methods

I plan to start with the RAVDESS dataset. This dataset appears to have some advantages over the TESS. The RAVDESS is 
gender balancedand contains audio files from a larger group of actors. I may bring in the TESS dataset once I have a fairly
decent model trained on the RAVDESS.

The first step is to learn the python librosa library and figure out how to extract useful features from the dataset. Some
useful features may be pitch, volume, and talking speed. Some research may be necessary to identify more features to extract.

Once I have a grasp on feature engineering, I plan to make an MVP using only happy and sad audio files. Once this MVP
is working OK I'll expand the classifier to include other emotions. Given time, I may bring in the TESS dataset at this point
as well.

The final step of the project will be to deploy the classifier in a flask web app on either AWS or Heroku that allows users
to upload their own audio files. If possible it would be really cool if users could stream audio to the app and see it
work in real time, however this is likely beyond my abilities at the moment.
