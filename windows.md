=======
# DEFCON OBS Quickstart

## Windows Instructions

1. Download & install OBS for your platform: https://obsproject.com/
   1. Start OBS. Choose to run the auto-configuration wizard.
        1. Select __Optimize for Recording__, click next.
        1. As a base resolution, use 1920x1080.
   2. Open the application __Preferences/Settings__ to adjust some important settings:
        1. Under the __Output__ tab, under __Recording__ select:
            - __Recording Path__: `a path of your choice`
            - __Recording Quality__: *Indistingquishable Quality, Large File Size*
            - __Recording Format__: *mp4*
        2. Under the __Video__ tab:
            - Make sure both your __Base Canvas__ and __Output Resolution__ are set to `1920x1080`
        3. Click __OK__ to exit and save the changes

### Get & Configure The Template

OBS does not support relative paths, operating-system-specific path specifiers (e.g. ~ or %USERPROFILE%) or pretty much anything else - this makes OBS templates an interesting problem. This is the fastest and easiest way to fix it.

1. Download the template and images for the main track: __LINK TO TEMPLATES HERE__
1. Unzip the templates zip file you downloaded to someplace where it can reside long term. This can be anywhere you like, as long as you know its path.
1. Open your text-editor of choice. Anything that does find and replace and understands UNIX line endings will do. When in doubt, Notepad++ is always a reasonable option.
1. Load the template configuration file - `dc-safemode-main-talks.json` 
1. Copy the path of the directory you created above (e.g. `c:\users\jack\Documents\dc-safemode-main-talks`), and replace the backslashes with slashes.
1. Using the Find/Replace feature of your text editor, find `%PATH_VAR%` and replace with your modified path (e.g. `c:/users/jack/Documents/dc-safemode-main-talks`) - this should fix all your file paths and ready you for importing the scenes.
1. Last but not least: add the included font `American Typewriter.ttf` to your system.

### Load The Template in OBS

1. Open OBS and select __Import__ from the __Scene Selection__ menu.
1. Click the the dots in the collection path to specify the JSON file inside the directory you specified earlier.
1. Click __Import__
1. From the __Scene Selection__ menu, choose `DC28SMTalks`.
1. Double-check to make sure images appear in the scenes you will be using. (This means the paths you added are correct!
1. There are two text overlay items for different platforms. 
    ![Platform Specific Text overlays](text-overlays.jpg)
1. On each one of the Scenes you intend to use, click the eye icon next to the MAC/LINUX text item to hide it. (It probably won't appear anyway, but on some configurations, might appear as garbled text.)
1. __Edit__ the overlay text on the WINDOWS item to add your name, talk name, or other title information.

At this point, you're ready to start adding audio & video to your configuration.

# Preparing For Recording 

### Audio Sources
High quality audio is imperative to having your video meet quality standards. Here are some suggestions for the best audio:
- Stand about 2-3 inches from the mic to avoid distorting your voice
- Avoid background noise like air conditioning (no AC on is preferred)
- Avoid filming outside or in noisy areas
- Test that your sound does not have echo. If it does, try a smaller room or more insulated space (closets work well)
- Your average recording volume should be between -12dB and -10dB. Check your levels on OBS by looking at the audio mixer panel.
- High quality mics help, using something like a laptop's built in mic can pick up a lot of fan noise. 
- If you need to normalize your audio, please do, [YouTube Audio Normalization](https://www.youtube.com/watch?v=OKSWPrT5upo)

### Live Video Sources
You will need to add a video source (or two) to each of the scenes you plan to use. Your first source will probably be yourself. Most presenters will probably be using a webcam or a phone, but there are many high resolution camera options available that work with OBS if you choose. Use something that shows you clearly. Lighting is more important than you think; you should be well-lit and use a background that contrasts your clothing so you appear clearly in the video.

Your second video source will likely be a screen recording or the screen of your computer for slides and or demos which you will record live. 

Regardless of which video source you choose, live or recorded, adding them will follow roughly the same instructions.
1. Select the scene you wish to use.
2. Under the sources pane, click the __+__ sign to add a source.
   - For capturing the screen, you would select __Display Capture__
   - For capturing a single window, you would select __Window Capture__
   - For capturing a webcam, you would select __Video Capture Device__
3. Resize each video source to the correct size to fit within the template 
    - The existing template items should already be locked in position. Once your items have been placed, you can also use the lock icon on those items to prevent them from being accidentally moved.
4. Check to ensure your video sources are listed at the bottom of the sources pane. This ensures they are "under" the template overlay and will inherit the same effects as other presenters
    
    ![DO THIS](do-this.png)
    ![DON'T DO THIS](do-not-do-this.png)

5. Resize and recenter your video after making sure it is under the template, it should appear to have horizontal stripes through the video and the edges of the video should look "torn" (see example)

### Let's Make A Test Reocrding

Once you have your video sources configured the way you want, they appear clearly in the preview window, and the audio level meter responds to your voice, you can try a test recording.

1. Click the __Start Recording__ option. 
    - You'll see a couple of visual cues, but in general, OBS does not have a lot of feedback during recording.
1. Record some test content. 
1. Click __Stop Recording.__

OBS places the recordings in the location you specified during the setup wizard, so you'll have to browse to that location and watch the video you just made. By default, they are named with the time and date you started recording. You'll want to peruse your test video to see how the audio sounds and how the video quality looks - if it all looks OK, you are good to record your full presentation.

**Note**: When you click __Start Recording__, a pause button appears. (You may have noticed this.) You can use pauses to make adjustments, change scenes, etc. as you go. 

**Note**: OBS supports __lots__ of different definable hotkeys for actions like starting/stopping/pausing recording, changing scenes and sources, etc. If you have something complex you'd like to do, you will most likely want to investigate the Hotkeys section in the OBS Settings dialog.

### NOTE: Pre-Recorded Video Sources
Fifty minutes is a long time if you make a mistake in your demo or have a technical difficulty and want to re-do it. During live DEFCONs mistakes are inevitable but for DEFCON SAFEMODE, people may want to fix these errors since they have the time. For this reason, you may think about doing a screen recording of the slides/demos which you can then narrate with audio and video afterwards, if you run into errors, you don't have to re-record quite so much. Or, if the audio isn't as clear as you'd hoped upon review, you don't have to re-record the slides, just the speaker video.