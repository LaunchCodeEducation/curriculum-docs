Making Lesson Videos
====================

Planning the Lesson
-------------------

A bit of preparation can go a long way toward making higher quality lessons while also reducing the time you spend re-recording or fixing mistakes. 

The basic components of planning the lesson are:

#. Define lesson objectives
#. Create an example or project that hits the objectives
#. Write an outline to follow while recording

Lesson Tips
^^^^^^^^^^^

**Go through the project yourself, in detail, before recording.** You might feel like you can wing it, but, even with simple examples, you put yourself at risk of stumbling across something you didn't plan on. There might be a project dependency you forgot you needed, or perhaps you forgot the API details for a library. Going through your lesson step-by-step before recording will result in a better end result.

**Make high-level process notes to serve as a script.** It can be easy to forget where you are, and what is next, when recording a lesson. Make a bullet-point list of the steps and keep it next to your computer for reference while recording. How detailed this outline should be is a matter of personal preference. 

**Keep it short, breaking the lesson into multiple steps if necessary.** Lesson videos should be less than 20 minutes total, and ideally less than 10 if the topic allows. If you're creating a longer lesson or project, break it up into logical sections. At the beginning of each section, remind the learner that the video is part of a larger series, and they should have viewed the earlier videos before beginning the current video.

Tech Setup and Recording
------------------------

Setup
^^^^^

.. note:: We currently only provide instructions for Mac computers. 

We'll use Quicktime and `Loopback <https://rogueamoeba.com/loopback/>`__ to record and route audio, respectively. You already have Quicktime, but you'll need to install Loopback.

.. note::

   Without paying for a Loopback license, audio quality will be
   degraded after 20 minutes. Keep recordings shorter than this (though
   you should be doing so for pedagogical reasons, anyway).

LaunchCode can lend you a recording kit for making a lesson. Your kit will contain:

-  Audiobox USB interface w/ USB cord
-  Microphone cable
-  Microphone
-  Headphones w/ ⅛" to ¼" adapter
-  Tabletop mic stand

Setting Up the Equipment
^^^^^^^^^^^^^^^^^^^^^^^^

1. Plug the USB cable into the back of the Audiobox, and plug the other end into your computer. Audiobox will now be available as an audio input device.
2. Plug in the mic cable to **Channel 1** (on the left) of the audiobox. Connect the other end of the mic cable to the microphone. 1 .Connect the headphones to the back of the Audiobox. If the ⅛" to ¼" adapter is not connected, you will not be able to do this. **Do not connect headphones to your computer**, as this will result in a delay between your speech and what you hear.
3. Adjust the knobs on the front of the Audiobox to match the following:

   -  Mic 1 level @ 4 o'clock
   -  Mic 2 level all the way down
   -  Headphone monitor level at a comfortable volume for you
   -  Mixer at 12 o'clock
   -  Main at 3 o'clock

.. image:: /_static/images/audiobox-setup.jpg
   :width: 600px

Setting Up the Software
^^^^^^^^^^^^^^^^^^^^^^^

1. Open Loopback and add a device from the left-hand menu. This new device will be a "virtual" audio source through which we'll route the mono/left channel microphone audio to a stereo output.
2. In the right-hand panel, select the + icon in the Source section and select Audiobox.

   .. image:: /_static/images/loopback-add-device.png
      :height: 400

3. In the bottom-right section, set Channel Mapping to Automatic. Then drag the Left (1) channel from the top section to both 1 (Left) and 2 (Right) output channels in the bottom section.

   .. image:: /_static/images/loopback-channel-mapping.png
      :width: 500px

4. Open Quicktime and select *File > New Screen Recording*.

   .. image:: /_static/images/quicktime-new-screen-recording.png
      :width: 500px

5. Select Audiobox as the audio source from the dropdown just right of the Record button.

   .. image:: /_static/images/quicktime-audio-source.png
      :width: 500px


Recording
^^^^^^^^^

Follow these steps to prepare for and make your lesson recording.

#. **Turn off notifications.** From the *Notification Center*, turn on *Do Not Disturb*. This will ensure that any system or message notifications are displayed while recording. You don't want embarrassing messages from a friend or spouse ending up in a lesson video!

   .. image:: /_static/images/mac-notifications.png
      :width: 300px

#. **Prepare your desktop.** Be aware of any personal info that might be visible, such as files on the desktop, bookmarks in your browser toolbar, open tabs, and so on. Remember, this video will be publicly available on the Internet. It's also a good idea to close down windows and apps that won't be in use during the lesson.

#. **Position the microphone.** Place the mic in the mic stand, and position the mic between you and your keyboard, between your arms. This is necessary for a good positioning distance for the mic. The mic should be 4-6 inches from your mouth. It should look like this:

   .. image:: /_static/images/mic-arrangement.jpg
      :width: 600px

#. **Test.** It is highly recommended that you make a short test recording to make sure everything was set up properly. Follow the steps below, record a few seconds of yourself talking, and watch it back. Make sure the audio sounds clear and has a good tone. If it doesn't, then you likely have the audio source in Quicktime set incorrectly.

#. **Start the recording.** Hit Record on Quicktime, then click anywhere on the screen to begin recording.

   Begin by introducing yourself and describing the lesson. You may use this intro as a template:

      "Hi, I'm (your name) with LaunchCode. In this lesson for (course name) we will (lesson overview)."

When you are done recording, click the Stop icon in the menu bar and save the video file.

Tips
----

-  It's okay to mess up. If you make a mistake, take a moment, make a note of what needs to be edited, back up, and continue.
-  It can be a good thing to work through an error or bug in the lesson; this normalizes the situation for learners. If learners only see you going through examples perfectly, with no mistakes, then they get the impression that more experienced developers never make mistakes.
-  As you go, describe what you are going to do at a high level before doing it. This helps learners understand the objective and follow along.
-  Create a branch or tag for the final (and, optionally, starting) code from the lesson to link to within the lesson page.

Publishing
----------

LaunchCode staff will take care of the hard work of editing and publishing your video.

1. Share the video with LaunchCode Education staff via Dropbox
2. Send an email to LaunchCode Education staff, including the following info for each video:

   -  File name
   -  Lesson title
   -  Description
   -  Editing notes

      -  Be as precise as possible, including specific timestamps for the sections in question.
      -  Are there sections that should be removed?
      -  Does the video need to be combined with another one?
