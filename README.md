# voiceClone
Description of Voice_Extration.ipynb
So initially, we have extracted the Audio from the Voice_Extraction file using python by moviepy. And then after converted the audio into the text form by Whisper
Now we're converting the English transcription into the Hindi transcrption using hugging module. 
Now from here we need to convert the text which is hindi to english in order for the model to understand.
Along with this process, we are generating the AI_speech which is in hindi. We are doing this step because, The Original Audio is in english and it's really hard for the model to extract the english language and use this information to talk in hindi. So, if we have a hindi speech, on how to pronounce the hindi alphabets and words. We can use this information to train the model and also, use the orginal english audio file, to get the accent of the speaker. 

Description of Voice_Cloning.ipynb
Now that we have the file according to our requirments. Now we are cloning the pre-trained model from the git hub.
After that we are giving it a destination, to deploy all the necessary files. 
Importing all the necessary packages such as ffmpeg, pytorch.
As we are doing this on google colab, we need to create the conda environment to sucessfully implement all the packages and run it, After that we are using !python demo_cli.py command in order to install all the require packages before install the other necessary files from the repository using the command pip install -r requirements.txt, such as, encoder, synthesis, vocoder.
Even after, this we may need to debugg the code in encoder/audio.py and encoder/interface.py as per our requirement. 
through the !python demo_cli.py we have sucessfully installed all the packages such as librosa, unidecode, inflect etc.
After we have completed this task we now have to lauch the software using the python demo_toolbox.py, and added additional packeages per requirements such as portaudio, umap etc. 
In the end as googlecolab is just a cloud interface it is unable to display the software SV2TTS, As it hardware isn't supported to dispaly qt.qpa.xcb and it's plugins though they were present in the files.
But, I have implement the whole process again in the Anconda prompt to establish the software SV2TTS. Now its successful, but sharing the code from the google co-lab.

Using the computer hardware we're able to succefully colne the model. We implemented the dataset of the speaker the audio of the speaker along with the transcription of the referenced audio to get the accent of the speaker in utterance box(19-198-0005.flac) and the same related files of the AI-speaking hindi audio (19-198-0006.flac) in the embaded box to get the prnounciation of hindi with the accent of the speaker from the original file.
Over synthesising the model for over 50 epchoes we are able to succefully get our desired Voice-cloning of the speaker. 
As my computer is not able to process the umap package we are unable to generate the clusters but we can generate the correlation table to determine the accuracy of our desired audio file. This can be used to determine the accuracy and all the output will be shared in the mail. 
