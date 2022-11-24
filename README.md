# Arcface 
## ai_ml Project
***
Hey! These are our codes and presentations for the ai_ml Deep Learning project.
We have made Arcface, which is the SOTA (State of the Art) face recognition model.<br>
[Link](https://arxiv.org/pdf/1804.06655.pdf) to paper.<br>
Links to all videos are present at the end of this document. It is recommended to watch the videos before trying out the code.
***
***
## Instructions to run Training Code
***
1. Create a python3 virtual environment in python3 or conda and download all the necessary libraries to make the project codes run. All required libraries are listed in the <b>requirements.txt.</b>
```console
@ai_ml_warrior: conda create --name arcface
@ai_ml_warrior: conda activate arcface
(arcface)@ai_ml_warrior: pip install -r requirements.txt
```
2. * The main training code in the <b>Codes</b> section of this folder is the python3 file named <b>arcface_training_code_v2.py</b>. 
    * The datasets for training are present in the folder named <b>datasets</b> inside <b>Codes</b> folder.
```console
@ai_ml_warrior: cd Codes
```
3. Activate the newly created venv with all neccessary libraries.
```console
@ai_ml_warrior: conda activate arcface
(arcface)@ai_ml_warrior: _
```
4. 
* Run the <b>arcface_training_code_v2.py</b> file to start training.
```console
(arcface)@ai_ml_warrior: python3 arcface_training_code_v2.py
```
* Else if you are comfortable with ipynb notebooks open the <b>Arcface_Training_Code_v2.ipynb</b> notebook, change the kernel to the created venv and execute the cells in order to start training.

5. Once the training reaches 50 epochs the model is saved in the <b>Codes</b> folder itself.<br>
***
***
## Instructions to run Vizualisations and Plots Code
***
1. Activate the newly created venv with all neccessary libraries.
```console
@ai_ml_warrior: conda activate arcface
(arcface)@ai_ml_warrior: _
```
2. 
* Run the <b>arcface_visualizations.py</b> file to calculate threshold and create the plots.
```console
(arcface)@ai_ml_warrior: python3 arcface_visualizations.py
```
* Else if you are comfortable with ipynb notebooks open the <b>Arcface_Visualizations.ipynb</b> notebook, change the kernel to the created venv and execute the cells in order to calculate threshold and create the plots.

A) Executing ipynb notebook is preferred in this case.<br>
***
***
## Instructions to run Face Verification Code
***
1. Activate the newly created venv with all neccessary libraries.
```console
@ai_ml_warrior: conda activate arcface
(arcface)@ai_ml_warrior: _
```
2. * Images are stored in the images folder. 
    * Upload images you wish to verify. (make sure they are closely cropped images of faces.
    * Change path in line 152,153 in <b>arcface_face_verification.py</b> or the 5th cell in <b>Arcface_Face_Verification.ipynb</b> for face verification with paths to different images if you wish to.
3. 
* Run the <b>arcface_face_verification.py</b> file to verify.
```console
(arcface)@ai_ml_warrior: python3 arcface_face_verification.py
```
* Else if you are comfortable with ipynb notebooks open the <b>Arcface_Face_Verification.ipynb</b> notebook, change the kernel to the created venv and execute the cells in order to load model then verify if both are the same people or not.

A) Executing ipynb notebook is preferred in this case.<br>
B) In this file, a Resnet-34 model is used as a backbone. We trained it to reduce model size for our flask deployment, but it wasn't significantly smaller than our Resnet-50 backbone arcface model.<br>
***
***
## Instructions to run Face Verification Deployment with Gradio
***
1. Activate the newly created venv with all neccessary libraries.
```console
@ai_ml_warrior: conda activate arcface
(arcface)@ai_ml_warrior: _
```
2. Run the <b>gradio_dep.py</b> file to start the server.
```console
(arcface)@ai_ml_warrior: python3 gradio_dep.py
```
```
3. Run the app.py file to start the server.
```console
(arcface)@ai_ml_warrior: python3 app.py
ArcFace expects  []  inputs
and it represents faces as  (512,)  dimensional vectors
Running on local URL:  http://127.0.0.1:7860
Running on public URL: https://90d977e0e66***20.gradio.app
```
4. Copy the address in which the server is running and open it on your default browser.
5. * Once you select image 1 and image 2, don't forget to upload them before trying to verify if they are the same people.
***
***
## Other Links
***
- [Paper Review Log](https://zestyoreo9.gitbook.io/deep-learning-and-neural-networks/one-shot-learning-project/papers)<br>
- [Connected Papers.com](https://www.connectedpapers.com/main/d4f100ca5edfe53b562f1d170b2c48939bab0e27/ArcFace%3A-Additive-Angular-Margin-Loss-for-Deep-Face-Recognition/graph)<br>
- [Main Github Repo](https://github.com/zestyoreo/Arcface)<br>
- [Presentation Link](https://iitbacin-my.sharepoint.com/:p:/g/personal/200050103_iitb_ac_in/EbD_mES0PHtAkZ0ljE6R_GEBHUDhEVAxVmAryNsBSrC21Q?e=mYMgmz)
***
***
## Project by <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2000501<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2002601<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2000500<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;20005010