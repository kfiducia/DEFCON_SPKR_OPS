# DEFCON OBS Quickstart

## macOS Instructions

1. Download & install OBS for your platform: https://obsproject.com/
   1. Select the __Optimize for Recording__ option when asked
   2. Open the application __Preferences/Settings__ to adjust some important settings:
         1. Under the __Output__ tab, under __Recording__ select:
            - __Recording Quality__: *Indistingquishable Quality, Large File Size*
            - __Recording Format__: *mp4*
            - __Recording Path__: `a path of your choice`
        2. Go to the __Video__ tab on the left hand side
            - Make sure both your __Base Canvas__ and __Output Resolution__ are set to `1920x1080`
        3. Click __OK__ to exit and save the changes

2. Download the template and images for the main track: __LINK HERE__
3. Create a folder to house the template images, something like `~/Downloads/DEFCON_OBS/`
4. Open your text-editor of choice, if you don't have one, you can use the built-in `TextEdit.app`
5. Using the Find/Replace feature of your text editor, find `%PATH_VALUE%` and replace with your desired path e.g `/Users/username/Downloads/DEFCON_OBS/` - this should fix all your file paths and ready you for importing the scenes.
   - __NOTE:__ OBS does not seem to recognize the tilde character e.g. `~/Documents/`
6. Unzip the templates zip file you downloaded to the directory you specified above.
7. Open OBS and select __Import__ from the __Scene Selection__ menu.
8. Click the the dots in the collection path to specify the JSON file inside the directory you specified earlier.
9.  Change the __Name__ if you'd like to something you will recognize like `DEFCON-SAFEMODE`
10. Click __Import__
11. From the __Scene Selection__ menu, select the newly imported scenes.
12. Ensure the images appear in the scenes you will be using.
13. __Edit__ the overlay text to describe your specific talk in each scene you will use!
14. We will need to add/edit the video sources next. 


### Audio Sources
High quality audio is imperative to having your video meet quality standards. Here are some suggestions for the best audio:
- Stand about 2-3 inches from the mic to avoid distorting your voice
- Avoid background noise like air conditioning (no AC on is preferred)
- Avoid filming outside or in noisy areas
- Test that your sound does not have echo. If it does, try a smaller room or more insulated space (closets work well)
- Your average recording volume should be between -12dB and -10dB. Check your levels on OBS by looking at the audio mixer panel.
- High quality mic's help, using something like a laptop's built in mic can pick up a lot of fan noise. 
- If you need to normalize your audio, please do, [YouTube Audio Normalization](https://www.youtube.com/watch?v=OKSWPrT5upo)



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
    - EXAMPLE IMAGE DO/DONOT
5. Resize and recenter your video after making sure it is under the template, it should appear to have horizontal stripes through the video and the edges of the video should look "torn" (see example)


### Pre-Recorded Videos
Fifty minutes is a long time if you make a mistake in your demo or have a technical difficulty and want to re-do it. During live DEFCONs mistakes are inevitable but for DEFCON SAFEMODE, people may want to fix these errors since they have the time. For this reason, you may think about doing a screen recording of the slides/demos which you can then narrate with audio and video afterwards, if you run into errors, you don't have to re-record quite so much. Or, if the audio isn't as clear as you'd hoped upon review, you don't have to re-record the slides, just the speaker video.
    
