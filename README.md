# YOLOv4-COVID-restriction-monitoring

## About
Hi, my name is Hana and this is the code that was a part of my dissertation called ‘Monitoring social distancing and infection protection measures’. The code uses the computer vision YOLOv4 algorithm trained on images of people wearing masks, not wearing masks and wearing masks incorrectly to be able to detect these instances in images, videos and real-time camera footage. The Jupyter notebook also includes an app written in JavaScript, which includes a menu that lets you choose what you want to see detected in the video, short description of how to use the application and the detections on a real-life footage coming from your camera with additional options of detections you want to see.

Originally, I have planned to also add detection of certain types of masks, social distancing, number of people in a group restriction, curfews and following a one-way system. However, during the year I was writing my dissertation I ran out of time and decided to focus on improving the detection of mask wearing instead. Therefore, in the menu of an application there are still options of the other COVID restrictions, just in case of future development.

Additions to the code are welcome!

## How to run
This code has been stored in Google Drive and run in Google Colab, so if you want to run it on your machine remove the mounting to the Google Drive. Also download the ‘data’ folder from Google Drive at https://drive.google.com/drive/folders/1vATla0XRtkaMKcd2heHyQG54VuXvNxCa?usp=sharing which contains the photos and labels, if you are planning to also train and test the algorithm.

1. Create a folder 'yolov4mine' for your project and put the 'maincode.ipynb' file into it.
2. Open the maincode file and run steps above the 'change make file' label (the darknet folder should now be in the yolov4mine folder).
3. Download the 'yolov4-custom_best.weights' from this Google Drive https://drive.google.com/drive/folders/1yDsJ18eKdsSOsRjhLghuiPpRPOCVesoj?usp=sharing and put them into the backup folder.
4. In the darknet folder replace the 'Makefile', 'data' folder and 'cfg' folder folder with the objects of the same name from this git repo.
5. Run the 'change make file' and 'make make file' code to create the make file and the 'change cfg file' code.
6. Run the long code under 'on webcam recognition' and after approving the access to your camera, the application should appear on the bottom of the code.
