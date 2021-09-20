

# Tensorflow Object Detection For Building Detection

I have followed along the guide of Nicholas Renotte's Object Detection Course for creating a model for building detection in satellite images. I have made some small modifications for my ease, but most of the code is referenced from <a  href="https://github.com/nicknochnack/TFODCourse">his github</a>. I found this course really helpful. Here is his channel if you would like to go & support him: <a  href="https://www.youtube.com/c/nicholasrenotte">YouTube channel</a> &   <a  href="https://www.youtube.com/watch?v=yqkISICHH-U&t=5644s&ab_channel=NicholasRenotte">the course video</a>.

<img  src="https://i.imgur.com/BQ0ZQM1.jpg">

## Steps for using the model

<b>Step 0.</b> Download the pre-created virtual-env which contain the satDet & Tensorflow folders from this link as the files are large. Otherwise you can create a new one & train the model yourself.

<b>Step 1.</b> A virutal env named satDet is created which can be activated using 
<pre>
.\satDet\Scripts\activate
</pre>
and skip to 3 if you want to use the model directly.

OR
 
You can create your own but will need to install requirements again and move to step 2.
<br/>
<b>Step 2.</b> Install dependencies and add virtual environment to the Python Kernel
<pre>

python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=venv_name

</pre>

<br/>
<b>Step 3.</b> Go through collect.ipynb if you have created a new venv. Else you can add your images to rand folder under

<pre>
Tensorflow\workspace\images\rand
</pre>
and skip to step 5.
<br/>

<b>Step 4.</b> Begin training process by going through train.ipynb, 
Use the error guide here <a  href="https://github.com/nicknochnack/TFODCourse/blob/main/README.md">Error Guide.md</a>. Other errors may need some searching of your own.
<br/>
<b>Step 5.</b> You can run detect.ipynb which will run the precreated model for all the images under rand folder. 


If you want to improve the model, you can add more images with collect.ipynb and train it again for more steps.  Currently the model has achieved it's maximum capacity as learning rate is 0 after 50,000 steps.

For 18 images, it took 2886 object creation in labels so a lot of manual labor is required. You have been warned.

Thank you!
