# DeepFake-Creation-Using-DeepFace-Lab

#This readme.txt file is for the project "A survey of deepfake creation and detection.

Following the instructions here, you can create face swap deepfakes videos using DeepFaceLab.

DeepFaceLab is a state-of-the-art framework for realistic face-swapping results. DeepFaceLab is flexible to use and provide better results with high-efficiency components and tools.

# Training via NVIDIA or AMD GPUs.


Step1.## Installation
	 Install the compatible version of DeepFace Lab from link https://mega.nz/folder/Po0nGQrA#dbbttiNWojCt8jzD4xYaPw.

Step2.## Data uploading
 	Set your DeepFaceLab by uploading data_src (video that will be used for the replacement) and data_dst videos (video that will be replaced with the source video) as uploaded in the workspace folder. 

Step3.## Pre-processing
	 - Use the extract images from the video data_src and data_dst scripts to extract images from the data_src and data_dst videos and store this pre-processed data in separate folders. 
 	 - Use the data_dst and data_src extract faces S3FD best GPU scripts to extract faces from the data_src and data_dst videos and store them in data_src and data_dst folders. 

Step4.##Training
	Use training scripts to train your model via different settings used in modelname_summary.txt files in each model folder.

Step6.## Conversion
 	A convert script will swap (source to destination) faces in each frame. Also, if needed, use several productivity tools. 

Step7.## Result
	 Use convert mp4 lossless format to achieve a face swap deepfake video. 

#Training via Google Colaboratory Pro

More or less, it's the same procedure as using CLI of DeepFaceLab, but Google Colaboratory provides more GPU power to speed up the process.

User can train fakes for free using Google Colab at https://github.com/chervonij/DFL-Colab.

Step1.## Pre-processing
	 Follow the first three steps mentioned above for pre-processing and make a workspace.zip file to upload all pre-processed data to Google drive. 

Step2.## Installation
	 - Install DeepFaceLab in Google Colaboratory environment through cloning. 
	 - Import workspace.zip file from google drive. 

Step4.##Training
	Train your model using SAEHD and Quick96 configuration in Google Colaboratory environment with the different settings also mentioned in modelname_summary.txt files in each model folder.

Step5.## Conversion
	 Use merge script to swap (source to destination) faces.

Step6.## Result
Use result video mode to concatenate the frames to obtain face swap deepfake. 

