# Detect-and-recognize-Vietnamese-data-on-car-registration-by-MMOCR-and-PaddleOCR
A project to test model Paddle and MMOCR to read car registration photos
A quick description of how the project works.
Step 1: A little basic image processing before infer model.
- Adjust brightness and contrast to make text pop (openCV)
- Scan the image by segmenting the document using the MobilenetV3-Large model, then determine the 4 corners and flip the image using OpenCV.
- ![image](https://github.com/nndang27/Detect-and-recognize-Vietnamese-data-on-car-registration-by-MMOCR-and-PaddleOCR/assets/97721662/6896e978-60a2-448c-803e-ac72573a677d)
![image](https://github.com/nndang27/Detect-and-recognize-Vietnamese-data-on-car-registration-by-MMOCR-and-PaddleOCR/assets/97721662/4f724929-e31c-4133-a55d-12a1dd015d9b)
