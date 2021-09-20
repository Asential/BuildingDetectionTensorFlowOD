

# Tensorflow Object Detection For Building Detection

I have followed along the guide of Nicholas Renotte's Object Detection Course for creating a model for building detection in satellite images. I have made some small modifications for my ease, but most of the code is referenced from <a  href="https://github.com/nicknochnack/TFODCourse">his github</a>. I found this course really helpful. Here is his channel if you would like to go & support him: <a  href="https://www.youtube.com/c/nicholasrenotte">YouTube channel</a> &   <a  href="https://www.youtube.com/watch?v=yqkISICHH-U&t=5644s&ab_channel=NicholasRenotte">the course video</a>.

PDF for more details about the model: <a  href="https://drive.google.com/file/d/1KOKTNuf5NpicktgXd4a7sCuK5Pgdj4DW/view?usp=sharing">Overview PDF</a> 

<img  src="https://i.imgur.com/BQ0ZQM1.jpg">

## Steps for using the model

<b>Step 1.</b> You can use the pre-trained model my_ssd_mobnet by copying it in the Tensorflow/workspace/models/ directory after creating the virtual env directory & Tensorflow directory in train.ipynb OR create a new one & train the model yourself.
 
<br/>
<b>Step 2.</b> Create an virutal env, install dependencies and add virtual environment to the Python Kernel
<pre>

python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=venv_name

</pre>

<br/>
<b>Step 3.</b> Go through collect.ipynb if you are training the model again. Else you can add your images in a the directory:

<pre>
Tensorflow\workspace\images\rand
</pre>

and skip to step 5.

At any step if directory isn't present, you can go through the notebooks in order to create them 

- collect.ipynb
- train.ipynb
- detect.ipynb

<br/>

<b>Step 4.</b> Begin training process by going through train.ipynb, 
Use the error guide here <a  href="https://github.com/nicknochnack/TFODCourse/blob/main/README.md">Error Guide.md</a>. Other errors may need some searching of your own.
<br/>
<b>Step 5.</b> You can run detect.ipynb which will run the precreated model for all the images under rand folder. 


If you want to improve the model, you can add more images with collect.ipynb and train it again for more steps.  Currently the model has achieved it's maximum capacity as learning rate is 0 after 50,000 steps.

For 18 images, it took 2886 object creation in labels so a lot of manual labor is required. You have been warned.

Thank you!
