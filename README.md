

webcam-pulse-detector
-----------------------


How it works:
-----------------
This application uses [OpenCV](http://opencv.org/) to find the location of the user's face, then isolate the forehead region. Data is collected
from this location over time to estimate the user's heart rate. This is done by measuring average optical
intensity in the forehead location, in the subimage's green channel alone (a better color mixing ratio may exist, but the 
blue channel tends to be very noisy).
Once the user's heart rate has been estimated, real-time phase variation associated with this 
frequency is also computed. This allows for the heartbeat to be exaggerated in the post-process frame rendering, 
causing the highlighted forehead location to pulse in sync with the user's own heartbeat.


Requirements:
---------------

- [Python v2.7 or v3.5+)](http://python.org/)
- [OpenCV v2+](http://opencv.org/)
- Numpy, Scipy


