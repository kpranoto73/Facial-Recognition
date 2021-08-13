# Facial-Recognition

Description: The program would use image stored in a library to compare with video camera from a webcam to check if it is the same person. 

Important: This program was run on a Mac, windows hasn’t been tested and the release of the program doesn’t work so it would go to error when you want to close it. I force close it and restart the program to end it. 

Program Flow:
The program would require the import of face_recognition, cv2, bumpy and matplotlib. First, you would need to load the images using the facial_recognition.load_image_file and face_encoding to encode the faces from the images. You would repeat the process for all the people you want to be identified with the webcam. Next, you would need to store all the face encoding towards a list of facial encoding at the same time a known face name that correspond and is parallel in positioning with the face encoding. Then, some variables face_location, face_encoding, face_names, process_this_frame for the loop. This part of the program is the long part and would take time to load up all the images, the rest of the program would run on the go.

First, start with the video_capture from cv2 to load the camera and use a while loop to keep the facial recognition running. Video_capture.read() would take a single frame and check it against the database that is established. Small_frame would resize the frame of the idea camera and images for comparison would require conversion from BGR to RBG. face_recognition.face_location would locate the faces in the video camera and face encoding would encode the faces. The next for loop would math the faces from known face encoding with the face encoding taken from the video camera, if there is a match, it would be labeled and f not it would be labeled unknown. Next, the program would form a box around the face, drawing it and showing it on the video camera. 

NOTE: This program was run on a Macbook Laptop with the webcam. Known people are the example of 2 people with multiple photo used as a reference and compare with the video camera feed. This means if the person in the video camera feed are available in the known people folder, then the program will recognize them and label them with the corresponding name in the program
