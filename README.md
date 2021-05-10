# Assignment #5 Setup Instructions
** Please note: Do not post your code/assignments publicly.**

The goal of this assignment is to give you hands-on experience with various techniques for generating images using computer vision + machine learning (CVML) techniques… with dogs.

## Step #0 Use Google Colab
For a variety of reasons, this assignment is more approachable using Google Colab (Google's version of Jupyter notebooks). Instructions below assume use of Google Colab. However, this assignment has been set-up so you should not need to upload any external data files, so everything should be ready to run.

## Step #1 Watch the Google Colab instructional video
If you haven't already, make sure you watch the Google Colab instructional video, linked in the Glow assignment.

## Step #2 Ensure you have all programming modules
This week, our installation could be a bit tricky. The code to install and import everything you need is already in the Google Colab. We need:
* _scikit-image_ # `!pip install scikit-image`
* _tensorflow 1.15)_ # `!pip install tensorflow==1.15`
  * If getting this error: `ERROR: Could not find a version that satisfies the requirement tensorflow==1.15`, you likely have python version 3.8 or later, which requires tensorflow 2.2 or later (Iris is using Python 3.6.4). You may need to downgrade your python version.  (we can enforce the Python version in Google Colab by clicking Runtime -> Change Runtime Type).
* _tensorflow_hub_ # `!pip install tensorflow_hub`
* _opencv-python_ # `!pip install opencv-python`

We'll also need to import additional modules available in Google Colab, including: BytesIO, IPython.display, numpy, urllib, PIL, scipy.stats, scipy.misc, requests, tqdm, random, and cv2. 

## Step #3 Access homework files via Google Colab
You can access any public GitHub Jupyter Notebook on Google Colab by replacing the `github.com` in the URL with `colab.research.google.com/github`, like so: `[https://colab.research.google.com/github/UberHowley/haii-a5/blob/main/Dog_Image_Generation.ipynb](https://colab.research.google.com/github/UberHowley/haii-a5/blob/main/Dog_Image_Generation.ipynb)`.

## Step #4 Jump through the Google hoops
If you've watched the Google Colab instructional video, you know there's a couple hiccups to get through before you can work on the Colab. Follow those steps, and you should be ready to get going! Remember:
* Google Colab has a tendency to 'collapse' cells, make sure you uncollapse all the cells!
* Your runtime will expire when you idle, making it so you have to re-run all your cells, so try not to idle at an inconvenient place in the notebook. Much of this code can take a long time to run!
* Save often!
* You can export your Google Colab as a `.ipynb` file!

## Step #5 Get going!
Follow the instructions within the notebook. Remember, the course disucssion forums and Student Help Hours are there to help you out!

## Step #6 Turn it in
Once you've completed all of the above, you're done with this project! As always, clean up your code and ensure your entire Notebook runs before submitting, Iris must be able to run your notebook on her machine.

Once you think everything is set, export your Colab as a .ipnyb, and please set the filename to `[yourunixID]_haii21[assignmentnumber].ipynb`, e.g., `ikh1_haii21a5.ipynb` and then submit your notebook via Glow.

# Google Colab
If you haven't used Google Colab before, a good first step for you would be to read [Google's Welcome to Colaboratory](https://colab.research.google.com/notebooks/intro.ipynb?utm_source=scs-index) and take the User Interface Tour in the Jupyter notebook Help menu once you've opened your first Jupyter Notebook.

# Resources
- General resources: 
    * [Google's Welcome to Colaboratory](https://colab.research.google.com/notebooks/intro.ipynb?utm_source=scs-index)
    * [Python3 Documentation](https://docs.python.org/3/index.html) (tutorial and library reference are likely useful)
    * Python tutorials from [w3schools](https://www.w3schools.com/python/) and [Scrimba](https://scrimba.com/learn/python).
- [ImageNet](http://www.image-net.org/)
- Tensorflow:
  * [tensorflow](https://www.tensorflow.org/)
- bigGAN:
  * [bigGAN](https://tfhub.dev/deepmind/biggan-128/2)
  * [bigGAN tutorial](https://colab.research.google.com/drive/1rqDwIddy0eunhhV8yrznG4SNiB5XWFJJ)
    * [Machine Learning for Artists](https://ml4a.github.io/)
  * [tensorflow's Generating Images with bigGAN](https://www.tensorflow.org/hub/tutorials/biggan_generation_with_tf_hub)
