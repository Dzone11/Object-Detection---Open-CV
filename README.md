# Object-Detection - OpenCV
This project is about object detection using OpenCV, a popular computer vision library.

This is a brief description of the project that I have done on object detection using OpenCV. The main steps are:

- I downloaded the 'ssd_mobilenet_v3_large_coco_2020_01_14' model from the TensorFlow model zoo, which is a pre-trained model for object detection based on the Single Shot Detector (SSD) architecture and MobileNetV3 backbone.
- I extracted the 'frozen_inference_graph.pb' file from the model, which contains the model's weights and graph definition.
- I loaded the 'frozen_inference_graph.pb' file into opencv using the cv2.dnn.readNetFromTensorflow function, which returns a network object that can perform inference on images or videos.
- I used the cv2.dnn.blobFromImage function to preprocess the input images or frames, which resizes them to a fixed size, subtracts the mean values and optionally swaps the color channels.
- I used the network object's setInput and forward functions to feed the input blob to the model and get the output detections, a list of bounding boxes, class labels, and confidence scores for each detected object.
- I used the cv2.rectangle and cv2.putText functions to draw the bounding boxes and labels on the original images or frames and displayed them using cv2.imshow or saved them using cv2.imwrite or cv2.VideoWriter.
- I also used the cv2.VideoCapture functions to capture video from a webcam and apply the same steps as above to perform real-time object detection.
  
You can choose use your own jpeg and mp4 file for detection.
I have also uploaded the files that i have used.
