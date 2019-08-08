# Voice_Emotion
### Detecting emotion in voices  
  
## Intro  
  
Human expression and communication is multi-faceted and complex. For example, a speaker
not only communicates through words, but also through cadence, intonation, facial
expressions, and body language. It's why we prefer to hold business meetings in person
rather than over conference calls, and why conference calls are preffered over emails or texting.
The closer we are the more communication bandwidth exists.

Voice recognition software has advanced greatly in recent years. This technology 
now does an excellent job of recognizing phoenetic sounds and piecing these together 
to reproduce spoken words and sentences. However, simply translating speech to text does not
fully encapsulate a speakers message. Facial expressions and body language aside, text 
is highly limited in its capacity to capture emotional intent. It's why sarcasm is so
difficult to capture on paper.  
  
This github repo contains code used to build, train, and test a convolutional neural network to
classify emotion in input audio files.  
  
## Data
  
Data for training and testing this classifier was obtained from three University compiled
datasets: RAVDESS, TESS, and SAVEE. In total these datasets provide > 4,000 labeled audio files
across 7 common emotional categories (neutral, happy, sad, angry, fearful, disgusted, surprised)
spoken by 30 actors. 
  
The RAVDESS audio files are easily available online in a single downloadable zip file.
The TESS files are also easily available but require some web-scraping and a `wget`
command in order to avoid downloading > 2,000 files individually. The SAVEE files require
registration to access, anyone can easily register. Once registered the files can be easily
downloaded via a single `wget` command.
