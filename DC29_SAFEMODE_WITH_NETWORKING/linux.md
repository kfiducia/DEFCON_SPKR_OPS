# DEFCON OBS Quickstart

## Linux Instructions

Linux installation instructions for OBS Studio are maintained by the OBS Project and can be found on the [OBS Wiki](https://obsproject.com/wiki/install-instructions). 

Official installation packages are available only for Ubuntu 18.04, but unofficial installation instructions are available on the wiki for _many_ different distributions. Please complete the installation 

### Configuring Your Installed OBS Studio

Linux installations will require some additional settings that other distributions normally configure in the installer.

1. Open OBS Studio, and click the Settings button in the lower right.
2. Output section -> Streaming:
    1. __Video bitrate__: 2500 kbps
    2. __Encoder__: If you have a hardware option here, you may want to choose it. Otherwise, leave Software.
    3. __Audio Bitrate__: 128
3. Output section -> Recording: 
    1. __Recording Quality__: *Indistingquishable Quality, Large File Size*
    2. __Recording Format__: *mp4*
    3. __Recording Path__: `a path of your choice`
4. Video section:
    1. Make sure both your __Base Canvas__ and __Output Resolution__ are set to `1920x1080`
    2. Click __OK__ to exit and save the changes

5. Download the OBS/Linux specific template and image bundle from Basecamp.
6. Create a folder to house the template images. This can be anywhere you like, so long as you know the full path to it.
7. Open your text-editor of choice.
8. Using the Find/Replace feature of your text editor, find `%PATH_VALUE%` and replace with your desired path e.g `/home/username/downloads/DEFCON29` - this should fix all your file paths and ready you for importing the scenes.
   - __NOTE:__ OBS does not support any kind of relative pathing, or any path replacement variables (dots, %, etc.) You'll need to use a full, complete path.
9. Unzip the templates zip file you downloaded to the directory you specified above.
10. Install the Futura Font included in the template .zip
11. Open OBS and select __Import__ from the __Scene Selection__ menu.
12. Click the the dots in the collection path to specify the JSON file inside the directory you specified earlier.
13. Change the __Name__ if you'd like to something you will recognize like `DEFCON29`
14. Click __Import__
15. From the __Scene Selection__ menu, select the newly imported scenes.
16. Ensure the images appear in the scenes you will be using.
17. __Edit__ the overlay text to describe your specific talk in each scene you will use!
18. We will need to add/edit the video sources next. 

### Audio Sources
High quality audio is imperative to having your video meet quality standards. Here are some suggestions for the best audio:
- Stand about 2-3 inches from the mic to avoid distorting your voice
- Avoid background noise like air conditioning (no AC on is preferred)
- Avoid filming outside or in noisy areas
- Test that your sound does not have echo. If it does, try a smaller room or more insulated space (closets work well)
- Your average recording volume should be between -12dB and -10dB. Check your levels on OBS by looking at the audio mixer panel.
- High quality mic's help, using something like a laptop's built in mic can pick up a lot of fan noise. 
- Use a foam covering or pop filter on your microphone if possible
- If you need to normalize your audio, please do:
   Normalization is an audio editing process that helps all of our videos stay on the same relative volume. Normalizing the audio ensures when someone streams your talk the audio will be at the same level as the other talks. There are many ways to normalize audio, here is one method using Audacity, which is a free, open source, cross-platform audio software.
   1. Export the audio track from your video and open it with Audacity
   2. Select “Effect” then “Normalize…”
   3. Only have the second box selected and set the maximum amplitude to “-.1DB”
   4. Export the edited audio and re-add it to OBS as an audio source or re-attach to your video
      - Try to minimize the number of compression cycles the audio goes through or use the maximum quality available so the audio isn't degraded in this process.
   


### Live Video Sources
You will need to add a video source (or two) to each of the scenes you plan to use, you can search the internet for good quality cameras for video, but you may also be able to use your phone or webcam as a video source for this purpose. Use something that shows you clearly. You should be well-lit and use a background that contrasts your clothing so you appear clearly in the video.

Your second video source will likely be a screen recording or the screen of your computer for slides and or demos which you will record live. 

Regardless of which video source you choose, live or recorded, adding them will follow roughly the same instructions.
1. Select the scene you wish to use.
2. Under the sources pane, click the __+__ sign to add a source.
   - For capturing the screen, you would select __Display Capture__
   - For capturing a webcam, you would select __Video Capture Device__
3. Resize each video source to the correct size to fit within the template 
    - You may need to lock the template images/text to avoid accidentally moving or resizing the template
4. Check to ensure your video sources are listed at the bottom of the sources pane. This ensures they are "under" the template overlay and will inherit the same effects as other presenters
5. Resize and recenter your video after making sure it is under the template, it should appear to have horizontal stripes through the video and the edges of the video should look "torn" (see example)


### Pre-Recorded Video Sources
Fifty minutes is a long time if you make a mistake in your demo or have a technical difficulty and want to re-do it. During live DEFCONs mistakes are inevitable but for recorded DEFCON talks, people may want to fix these errors since they have the time. For this reason, you may think about doing a screen recording of the slides/demos which you can then narrate with audio and video afterwards, if you run into errors, you don't have to re-record quite so much. Or, if the audio isn't as clear as you'd hoped upon review, you don't have to re-record the slides, just the speaker video.

    

