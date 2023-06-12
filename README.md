# Detect-and-recognize-Vietnamese-data-on-car-registration-by-MMOCR-and-PaddleOCR
A project to test model Paddle and MMOCR to read car registration photos
A quick description of how the project works.

Step 1: A little basic image processing before infer model.
- Adjust brightness and contrast to make text pop (openCV)
- Scan the image by segmenting the document using the MobilenetV3-Large model, then determine the 4 corners and flip the image using OpenCV.
- ![image](https://github.com/nndang27/Detect-and-recognize-Vietnamese-data-on-car-registration-by-MMOCR-and-PaddleOCR/assets/97721662/6896e978-60a2-448c-803e-ac72573a677d)
![image](https://github.com/nndang27/Detect-and-recognize-Vietnamese-data-on-car-registration-by-MMOCR-and-PaddleOCR/assets/97721662/4f724929-e31c-4133-a55d-12a1dd015d9b)

Step 2: Detect and split each word directly using the inference model of SAST by PaddlePaddle
![image](https://github.com/nndang27/Detect-and-recognize-Vietnamese-data-on-car-registration-by-MMOCR-and-PaddleOCR/assets/97721662/bdced1ce-c8b6-473f-859d-968b28585dd2)
Step 3: Generate about 10000 sample images using for MMOCR training by https://github.com/Belval/TextRecognitionDataGenerator
![image](https://github.com/nndang27/Detect-and-recognize-Vietnamese-data-on-car-registration-by-MMOCR-and-PaddleOCR/assets/97721662/785e38be-3745-4802-b06c-224d510bd797)
Step 4: Training model MMOCR 
The obtained result is quite positive 🤭
![image](https://github.com/nndang27/Detect-and-recognize-Vietnamese-data-on-car-registration-by-MMOCR-and-PaddleOCR/assets/97721662/1ec01822-1eb4-4d38-8772-601f51e1db56)
Step 5: Write code rules to link words in output to a meaningful sentence or long word and specific metrics about car registration 
![image](https://github.com/nndang27/Detect-and-recognize-Vietnamese-data-on-car-registration-by-MMOCR-and-PaddleOCR/assets/97721662/081744a1-cf09-454d-a962-7c18626ca08d)
