# MultiCamFBT
An attempt at multi camera trackerless full body tracking for vrchat or other vr games

Here are the goals of the project, they are subject to change at any time. Read on to see an outline of how the program works.

Current goals:
-Support for 3 cameras that can all see each other
-Trackerless support only
-Wired USB camera support only
-Support for certain cameras only ? (this is to be better defined during initial development)
-Minimal smoothing and motion prediction
-openxr on Linux support
-Mostly Python -proof-of-concept- implementation (should be fast enough, just not ideal)

Intermediate goals:
-Standalone support (with an independent PC to process camera feeds)
-C++ implementation (I do struggle with build systems so this will be quite a jump)

Future goals:
 - steamVR support
 - Windows support (will likely require contributors, so could be moved down in list)
 - Ability to use visual trackers like in AprilTag-Trackers
 - Ability to recieve input from slimevr trackers to sort of work with them to get their benefits (which are much higher sample rate than any camera could do) while preventing drift
 - More # cameras in order to cover a sort of whole-room setup
 - Support for IP and other camera inputs
 - More advanced smoothing and motion prediction that allows levaraging the advantages and weaknesses of multiple types of cameras:  
  - the greater precision that higher resolution cameras will offer
  - more accurate motion offered by higher speed cameras
  - Taking latency into account for wireless or other higher-latency cameras -- a built-in tool to measure this latency

Indeterminant goals (mostly ML stuff, stuff I'm not sure is possible, or stuff that massively exceeds my current skillset):
-Hand tracking
-Training a pose predictor that takes more data into account that is useful here -> perhaps looking at avatar to modify inputs to correspond more naturally between the person and their avatar
-ML-based motion prediction
-Support for IP cameras fully standalone (no accompanying PC required) <-This could be moved up depending on the pace of the project


