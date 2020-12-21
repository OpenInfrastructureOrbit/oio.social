---
layout: single
title: "rC3 Remote Streaming to OIO/A:F"
date: 2020-12-20 13:37:00 +0100
lang: en
toc: true
classes: wide
ref: rc3-remote-streaming
---

For rC3 we would like to offer you the possibility to connect so that you can hold your talks from home.

Please read this documentation and try out the tools described. If you have any questions, please contact us and let us test the setup together. Please also make yourself familiar with it if your talk is currently planned live on stage.

The selection of tools is based on the experience of several online events held this year.

## Architecture

1. transmission of camera image/sound and slides/other form of presentation to the OIO: OBS-Ninja
2. back channel and emergency communication in case of malfunction: BigBlueButton

![](/images/rc3-remote-streaming/obs-ninja.png)

![](/images/rc3-remote-streaming/bbb.png)

### BigBlueButton channel
BigBlueButton (BBB) is an open source software for online meetings. It requires no additional software installation and is best used in Chromium/Chrome.

### OBS-Ninja Desktop/Videoshare
Your content to director: OBS-Ninja is a browser streaming that does not require any app installation but only a current browser (Chromium/Chrome preferred).

## Procedure
Before the official launch of rC3, we would like to test the setup once with each of you. We will contact you to arrange an appointment.

The procedure is basically like this:

* you come 30 minutes before your talk to a defined BBB room, the foyer. The URL will be announced.
* a director angel will pick you up there and "take" you "to a hall". This will be a special BBB room just for this talk.
* Before your talk you will get two URLs for your browser.
  * **URL for Camera-Share**: You give this browser access to the webcam and microphone. You can then minimize the browser window.
  * URL for Slide/Desktop-Share**: Here you select either the window with the application you want to use for your presentation slides or the complete screen.
  * If you are more than one presenter or have more than one camera, e.g. if something is still being tinkered with under a document camera, there are as many URLs as you need until all participants and all cameras have been supplied.
  * If you have not received any URLs, we can set them up at the latest in the 30 minutes before the talk.
* If the technology works properly
    * We will wait together for the start of your talk according to the timetable.
    * A herald will introduce your talk, perhaps you will exchange a few words in the dialogue. Herald and director will be heard and possibly seen via BBB.
    * You simply give your talk, the director does the image mixing between the image sources (slides/speakers).
    * At every 10 min and 5 min remaining time you will get a short announcement from the director via BBB.
    * After your talk, the Herald will take over again and do the Q&A with the signal angel. Due to lack of audience on site, the questions will come from various channels on the internet.
    * There will be an opportunity to continue detailed discussions in a separate room after the talk has finished.

### A few tips at this point

* If you have slides with "video+sound inserts": **Chrome/Chromium** is the only browser that (to our knowledge) can currently reliably send audio "from the desktop". Moreover, it is a browser that at least partially succeeds in outsourcing video compression to existing hardware, such as CPU units or graphics card. This improves the picture quality considerably
* Please ** refrain from using GEMA-liable music** in your contributions.
* Microphone & audio setup deserve your attention: **headphones are an absolute requirement**, whether large headsets or small earbuds.
    * a **plug-in microphone** improves the sound, **headsets are even better**! The microphone in the laptop will probably not do a good job, as the fans often rev up when streaming video and this noise ends up in the audio stream
* **Light is important**: Make enough light that you can just see your laptop. Webcams are surprisingly low light compared to the cameras commonly found in phones
* **Remove fingerprints on the camera lens** beforehand. A cleaning cloth for glasses helps
* **Redshift** (often in combination with "Nightmode") does not look good in presentations.
* Please close all programmes that are not necessary during your talk. This will avoid pop-ups from messengers or notifications from other browser windows appearing during your presentation.
* If possible, use two monitors. Share one monitor and show your presentation. On the other monitor you can have other windows, e.g. the one with the back channel for the Herald and the director.
* If you have a **sophisticated camera setup** or even run a studio yourself: In OBS-Ninja you can also specify the virtual webcam as the source. Or an HDMI grabber with a video camera attached.
* **Recorded Talks** (pre-recording) and only "Q&A Live" is definitely an option if you are not sure that the internet bandwidth is sufficient and stable enough. Either as a "live on tape" recording in advance from a location with a better connection or you record yourself, e.g. with OBS. Corresponding slide layouts for split screen views will be available in the next 2-3 days.

# Details of the tools used
## OBS NINJA
To bring your presentation to the OIO/A:F stage we use OBS Ninja. This is a live streaming software that works purely in the browser and therefore does not require any additional software installation. We will send you two links. The channels will be password-protected to avoid uninvited visitors. Of course, you can also play with it yourself in advance and create your own rooms.

Please note that you will need two OBS-Ninja windows or tabs to use the webcam and to split the screen. OBS-Ninja currently runs best in Chromium/Chrome.

### Use an Invite link
Copy the link into your browser's address bar and enter the password.

![](/images/rc3-remote-streaming/obs-ninja-invite.png)
Unlock the screen and webcam.

### Open a room
Go to the VOC-OBS-Ninja page [OBS-Ninja](https://ninja.c3voc.de/) and start selecting/sharing screenshare and camera.

![](/images/rc3-remote-streaming/obs-ninja-raum-oeffnen.png)

### Set up webcam
To share the camera, the correct camera must now be selected and shared in the browser.
![](/images/rc3-remote-streaming/obs-ninja-webcam1.png)

Now there is a small preview image in which the view can be checked. The other settings should correspond to the previously selected settings in the browser.
![](/images/rc3-remote-streaming/obs-ninja-webcam2.png)

Start the stream by clicking on the start button.
![](/images/rc3-remote-streaming/obs-ninja-webcam3.png)

### Share screen
Select the desired screen and share it in the browser.

![](/images/rc3-remote-streaming/obs-ninja-screenshare1.png)

Confirm the selection and start the transmission with the share button.
![](/images/rc3-remote-streaming/obs-ninja-screenshare2.png)

Under MacOS, the screen sharing must be confirmed for the first time in Firefox.
![](/images/rc3-remote-streaming/obs-ninja-screenshare3.png)
Afterwards, Firefox must be restarted.
![](/images/rc3-remote-streaming/obs-ninja-screenshare4.png)

### Controls
There are controls under the video image that control the transmission.

On the left is a speech bubble that opens a chat window. The chat is visible to all participants.

Next to it is a loudspeaker symbol that can be used to stop the transmission of sounds from other programmes.

The third symbol from the left is a microphone with which the own microphone can be switched off.

Next to it is an eye with which the transmission can be switched to black so that the user's own screen or webcam can no longer be seen.

The cogwheel opens the stream settings in which, for example, other microphones can be selected or another screen for transmission.

On the far right is a red telephone with which the call/stream is ended.

![](/images/rc3-remote-streaming/obs-ninja-buttons.png)

## BigBlueButton

As a return channel to you, we use a room in BBB. Open it in another tab of your browser. Through this channel you will hear the moderation of the Herald and questions asked or instructions from the director.

We will send you a link to enter the room. Here, too, the first step is to give your permission for the microphone and, optionally, the camera.

The most important controls are in the middle. You can mute yourself by switching the microphone button. With the handset button you can stop audio transmission. The other buttons are for enabling camera or screen sharing.

![](/images/rc3-remote-streaming/bbb-bedienung.png)

# Test yourself
Here you can judge your image quality yourself, also depending on the selected maximum resolution and your usable Internet bandwidth.
Try it out yourself with different settings, preferably with two separate PCs on different internet connections, as the webRTC protocol used otherwise (ideally) does not go "through the internet" at all, but remains local, which does not show influences of e.g. available upload bandwidth.

* Speaker camera
    * Source PC: https://obs.ninja/?push=xJf8Mqs&room=test&hash=2e40&label=OIO_Test_Cam
        * (self-monitor/view: https://obs.ninja/?view=xJf8Mqs&scene&room=test&password=test123&label=OIO_Test_Cam)
* Speaker-Screenshare
    * Source PC: https://obs.ninja/?push=v2QAmBj&room=test&hash=2e40&label=OIO_Test_Screenshare
        * (self-monitor/view: https://obs.ninja/?view=v2QAmBj&scene&room=test&password=test123&label=OIO_Test_Screenshare)

again as a table, for easier clicking

Function | Transmitter | Receiver
---------|--------|----------
Speaker-Video | [source](https://obs.ninja/?push=xJf8Mqs&room=test&hash=2e40&label=OIO_Test_Cam) | [destination/monitor](https://obs.ninja/?view=xJf8Mqs&scene&room=test&password=test123&label=OIO_Test_Cam)
Speaker-Screenshare| [Source](https://obs.ninja/?push=v2QAmBj&room=test&hash=2e40&label=OIO_Test_Screenshare)| [Target/Monitor](https://obs.ninja/?view=v2QAmBj&scene&room=test&password=test123&label=OIO_Test_Screenshare)

## Test session / technical set-up rehearsal
We will test your setups with you in advance. You will receive an email for this or have already received one.

The main focus will be on the optimal settings for picture and audio quality. You don't have to have your talk ready for this!

If you have any questions or problems with the tools described above, please contact us as soon as possible.

# For your slides
## Layout
* No important details in the bottom right corner, if possible please.
(example image from 2019)
    * The camera image will possibly overlap the bottom right corner.
    * if you should have branding there, then it would be good if you could move it to the left or top. If you can't, then we won't use that view.
![](/images/rc3-remote-streaming/slides-example.png)
* Please create your presentations in 16:9 format, otherwise there will be black stripes at the borders.

## Artwork and Fonts
If you still want to design your slides according to the event theme, you can have a look at the style guide: https://howto.rc3.world/styleguide.html

## Tips & Tricks

Most operating systems have at least one option for displaying your webcam recordings. Before your talk, take a look at the picture from your camera and see if you are happy with it. Be aware of the lighting conditions at the time of your talk.
A camera check at noon with daylight is not meaningful if your talk takes place in the evening at 10 pm. It may be worthwhile to move a lamp to improve the light. But be careful that you are not overexposed and become a monochrome blur.

Make your background as neutral as possible and avoid personal items such as your birthday calendar, passwords or a clear line of sight into your neighbour's window.  The more boring your background is, the better.

The presentation style is significantly different this year than in previous years. There are no direct audience members and no immediate feedback from the audience. Make your presentation more personal by putting wiggle eyes, your favourite stuffed animal or a squeaky duck on/around/behind the camera. This way you can look the audience in the face more often and have a "real" audience at the same time, which often makes the presentation easier.

<small>Thanks to the [RheinRuhrStage](https://r3s.nrw/en), whose documentation we used as the basis for this article!</small>
