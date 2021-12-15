# Set Up

## Windows Mixed Reality

The first step to get started with the Headset Omnicept is to set up it withim the Windows Mixed Reality. All steps to do this are instructed in the [pdf](./Images/Headset_Set-Up.pdf)

## Runtime 

The Runtime is a system designed to connect the Headset sensors to applications running on a single PC. The download of the Runtime can be done at  https://developers.hp.com/omnicept/downloads, in the option "Omnicept Users", click at the button "Download latest HP Omnicept Runtime", as indicated in red at the following image:

![](/Instructions/Images/ButtonDownloadRuntime.png)

A new Web Page will load and the download will start automatically. If the download doesn't begin, verify if the browser blocked a pop up, click to allow the pop up:

![](/Instructions/Images/PopUpAllow.png)
 
and click at "Try downloading again":

![](/Instructions/Images/TryDownloadAgain.png)

After the download is completed, open the executable and follow the installation steps, at the final screen check the box "Woud you like to enable all your sensors?", and then click "Finish" :

![](/Instructions/Images/EnableSensors.png)

A request to "Restart" the system will appear to apply the runtime settings, click "Yes". After the system restarts the Runtime is ready.

## Eye Tracking Calibration

For the first time you use the Headset, it is necessary to calibrate the Eye Tracking sensor. To do this you have to execute the application "HP Omnicept Eye Tracking Calibration", wich was installed along with the Runtime, and can be found by searching for its name in the Windows Menu.

## Config File

### Initialisation

<span style="color:yellow">**WARNING**</span> you need to place the config file at the right location, if not you're will not be able to change parameters for the experiment.<br>

Open the startup menu by pressing the win key on your keyboard.

Type the following directory and press enter.    
> %appdata%\\..\LocalLow\

Create the remaining of the path 
> CERV\VR-PPE\  

Copy config.txt into the vr-ppe folder.<br>
Before starting the experiment fill up the config file with subject informations.<br>
At the end of the experiment you will get a folder named after the subject containing the raw data sensors and the result of the surveys.

### Parameters

**[userid]** is the section for the personnals informations of the subject it is hero to help you find the data afterward

* **name** you can write the full name of the subject and the output folder will be created after this name
* **age** just for statistics
* **health** you can report here any issues that might influence the experience
  
**[experiment]** is the section to modify the parameters of the experiment
* **type** this is where you can choose the type of experience
  * **calcul** : [Progressive Task](./instructions.md#progressive-task)
  * **doubleTask** : [Double Task](./instructions.md#double-task)
  * **tripleTaskNoInteruption** : [Triple Task](./instructions.md#triple-task)
  * **tripleTaskNASAtlx** : [Triple Task](./instructions.md#triple-task)
* **reverse** : Set it to **1** if you want to begin by the complex tasks work only with [Double Task](./instructions.md#double-task) and [Triple Task](./instructions.md#triple-task)
* **experienceTime** : Set the duration of each part of the experiment in seconds (default value = 180, 3 minutes for each part, 6 minutes in total)
* **pauseTime** : Set the duration of the pause between parts in seconds<br>
  <span style="color:yellow">**WARNING**</span> the **survey** wait to be confirmed even if it exceed pause time <br>
  (default value = 30)
* **survey** : displays a quiz derived from the NASA-TLX at the end of each part<br>answers are logged in a text file with the average response time and cognitive load by part
* **skipTuto** : allow you to skip the tutorial and begin with the experient right away.<br><span style="color:yellow">**WARNING**</span> the cognitive load start logging after one minute of play so if you skip the tutorial make sure to not start right away.
* **AudioStimulusAverage** : set the repetition rate for the audio stimulus in seconds (with 15 about 4 stimuli per minute).
* **AudioStimulusDelta** : set the maximus deviation from the average in seconds [average-delta , average+delta] (if set to 0 the stimulus will be constant).
* **MaximumResponseTime** : set maximum response time (time saved if there is no response from the user).
  
## Omnicept Sensor Diagnostic
To verify if the Headset sensors works there are an application for this. You can download the Omnicept Sensor Diagnostic at https://developers.hp.com/omnicept/downloads, scroll the page until the session tools, and you will find the download option. To download the application a HP Account is needed.

## Autorisations

After running the application for the first time a notification will appear requesting sensors permissions, **WARNING** if you do not accept the application will not save any data related to sensors

![](/Instructions/Images/Notification.png)

If you missed it don't worry you can access it by going into the hidden icons and open the omnicept runtime then in autorisation tab choost to trust the application by pressing ✔️.

![](/Instructions/Images/Runtime.png)

[Return to ReadMe](./../ReadMe.md)

[Go to instructions](./instructions.md) 

