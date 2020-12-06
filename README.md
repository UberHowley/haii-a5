# Assignment #5 Setup Instructions

## Step #1 Ensure you have all programming modules
This week, in addition to Anaconda Python 3.6 (or greater) with Jupyter Notebooks, you'll also need to install the following modules (maybe more, read your program output!):
* `tensorflow` 1.15 # pip install tensorflow==1.15
  * If getting this error: `ERROR: Could not find a version that satisfies the requirement tensorflow==1.15`, you likely have python version 3.8 or later, which requires tensorflow 2.2 or later (Iris is using Python 3.6.4). You may need to downgrade your python version (this would be a great use case for a [virtual environment in python](https://docs.python.org/3/tutorial/venv.html) or a [new anaconda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) with `conda create -n myenv python=3.6` and `source activate myenv`. You'll still need some extra steps to get Jupyter notebooks to use your environment `myenv`:
    * `pip install -- user ipykernel`
    * `python -m ipykernel install --user --name=myenv`
    * Then [change your kernel inside the Jupyter notebook to be `myenv`](https://medium.com/@nrk25693/how-to-add-your-conda-environment-to-your-jupyter-notebook-in-just-4-steps-abeab8b8d084)
  * If using Google Colab, will likely need `!pip install tensorflow==1.15` to specify which version of tensorflow to use.
* `tensorflow_hub` # pip install tensorflow_hub
* `skimage` # pip install scikit-image (possibly `pip install --upgrade scikit-image`)
  * If getting this error: `ERROR: Cannot uninstall '___'. It is a distutils installed project and thus we cannot accurately determine which files belong to it which would lead to only a partial uninstall.`, then the easiest approach might be to temporarily downgrade to pip version 9 (`pip install --upgrade --force-reinstall pip==9.0.3`) and then try again. If you don't wish to downgrade pip, then you'll need to manually go to site-packages and remove the module that cannot be uninstalled automatically and try upgrading again.
* `cv2` # pip install opencv-python
* `tqdm` # pip install tqdm
* `requests` # pip install requests

Install Anaconda Python 3.6-3.7 if you haven't already. [https://www.anaconda.com/distribution/](https://www.anaconda.com/distribution/) You'll need Jupyter Notebook, and scipy, at the very least.

## Step #2 Download homework files
Download all the files in this repository. Place these files into a well-named folder on your computer, and click on the zip file to unzip the data folder. You will zip all the files in this directory and submit the `.zip` file to Glow when completed.

## Step #3 (Terminal Option)
In your terminal, navigate to your homework folder and run `jupyter notebook .` to start the notebook. A notebook session should open up in your browser.

## Step #3 (Graphical User Interface Option)
Once Anaconda is installed on your machine, open an application called Anaconda-Navigator. On the main page, click the 'launch' button on the Jupyter Notebook tile. A notebook session should open up in your browser.

On Windows, you will do [something like this](https://pythonforundergradengineers.com/opening-a-jupyter-notebook-on-windows.html) by running the 'Anaconda Prompt' that comes with the Anaconda distribution.

## Step #4
Once you have the Jupyter Notebook for this assignment open, then follow the instructions described therein. 

# Jupyter Notebooks
If you haven't used Jupyter Notebooks before, a good first step for you would be to read the [Jupyter Notebook Tutorial: The Definitive Guide](https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook) and take the User Interface Tour in the Jupyter notebook Help menu once you've opened your first Jupyter Notebook.

# Resources
- General resources: 
    * [Jupyter Notebook Tutorial: The Definitive Guide](https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook)
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
