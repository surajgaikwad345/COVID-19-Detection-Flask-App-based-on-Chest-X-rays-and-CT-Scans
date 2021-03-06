# COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans
COVID-19 Detection based on Chest X-rays and CT Scans using four Transfer Learning algorithms: VGG16, ResNet50, InceptionV3, Xception. The models were trained for 500 epochs on around 1000 Chest X-rays and around 750 CT Scan images on Google Colab GPU. After training, the accuracies acheived for the model are as follows:
<pre>
                InceptionV3  VGG16   ResNet50   Xception
Chest X-rays    96%          94%      83%       92%

CT Scans        93%          93%      80%       95%
</pre>
A Flask App was later developed wherein user can upload Chest X-rays or CT Scans and get the output of possibility of COVID infection.

The article for the project was selected and published in <b>Towards Data Science</b>:<br> 
https://towardsdatascience.com/covid-19-detector-flask-app-based-on-chest-x-rays-and-ct-scans-using-deep-learning-a0db89e1ed2a

# Dataset
The dataset for the project was gathered from two sources:
1. Chest X-ray images (1000 images) were obtained from: https://github.com/ieee8023/covid-chestxray-dataset
2. CT Scan images (750 images) were obtained from: https://github.com/UCSD-AI4H/COVID-CT/tree/master/Data-split
80% of the images were used for training the models and the remaining 20% for testing

# Evaluation and Results
<h3>Sample output of test images</h3><br>

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/sample_chest.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/sample_ct.PNG">

<h3>Classification Reports for Chest X-rays:  VGG, InceptionV3, ResNet50, Xception </h3>

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/vgg_chest_report.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/inception_chest_report.PNG">

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/resnet_chest_report.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/xception_chest_report.PNG">

<h3>Confusion Matrix for Chest X-rays:  VGG, InceptionV3, ResNet50, Xception </h3>

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/vgg_chest_cm.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/inception_chest_cm.PNG">

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/resnet_chest_cm.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/xception_chest_cm.PNG">

<h3>Classification Reports for CT Scans:  VGG, InceptionV3, ResNet50, Xception </h3>

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/vgg_ct_report.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/inception_ct_report.PNG">

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/resnet_ct_report.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/flask%20app/assets/images/xception_ct_report.PNG">

<h3>Confusion Matrix for CT Scans:  VGG, InceptionV3, ResNet50, Xception </h3>

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/vgg_ct_cm.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/inception_ct_cm.PNG">

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/resnet_ct_cm.PNG"> <img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/xception_ct_cm.PNG">

<h3>Screenshots of Flask App</h3>

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/banner.PNG">

<img src="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/blob/master/screenshots/banner2.PNG" width="150%">

For more screenshots, please visit the <b>screenshots folder</b> of my repo, or <a href="https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans/tree/master/screenshots">click here</a>

<h3> How to use Flask App</h3>
<ul>
  <li>Download repo, change to directory of repo, go to command prompt and run <b>pip install -r requirements.txt</b></li>
  <li>On command prompt, run <b>python app.py</b></li>
  <li>Open your web browser and go to <b>127.0.0.1:5000</b> to access the Flask App</li>
</ul>

<h3> How to use Jupyter Notebooks </h3>
<ul>
  <li>Download my repo and upload the repo folder to your <b>Google Drive</b></li>
  <li>Go to the jupyter notebooks folder in my repo, right click the notebook you want to open and select <b>Open with Google Colab</b>   </li>
</ul>
