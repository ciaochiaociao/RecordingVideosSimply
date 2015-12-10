# RecordingVideosSimply

1. What about?
It is a simple practice for building an mobile native app in Java to use a built-in camera app to capture a video and to play the video taken inside my app. 

2. What for? 
A practice for intent concept and videoing. 

3. What features? 
It has two buttons: record and play. As record pressed, by sending inent, the app will open the built-in camera/video app in which all videoing procedure is done. After finishing, the captured result will theoretically be sent on onActivityResult() and the user then can  open the captured video by pressing Play button.

4. Current State: Doesn't work
As the video recording was finished, it came back to my app with "Unfortunately, Camera has stopped". And the play button didn't show anything.

5. As I was debugged...
At first moment, I used debugging tool and found out that the reason is the RESULT_OK in onActivityResult() being -1, which results from the operation failure of the app I sent intent to according to google android SDK guide. Also I thought maybe it's because of some problem of saving videos. But I'd checked that my video was certainly successfully taken and saved a place in my phone.

6. Main files
Java file: RecordingVideosSimply.java
Layout file: activity_recording_videos_simply.xml
Setting files: AndroidManifest.xml and build.gradle
