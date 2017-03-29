
# Example of Image Recognition using tensorflow/tflearn

Setup and installation of environment for osx. Will add information for 
linux soon. More details on setting up anaconda can be found here:
<http://machinelearningmastery.com/setup-python-environment-machine-learning-deep-learning-anaconda/>


### ANACONDA 4.3.1 
### Download and install conda:
```ANACONDA_NAME=Anaconda3-4.3.1-MacOSX-x86_64.sh
wget https://repo.continuum.io/archive/$ANACONDA_NAME
bash $ANACONDA_NAME
```

source ~/.bash_profile

conda create --name ml python=3.6
conda install conda-build

#Activate "ml" environment before installing packages
#Remember to look for the (ml) infront of computer$ in your terminal
#to verify that the environment is activated.
source activate ml

pip install jupyter
pip install scikit-learn
pip install matplotlib
pip install tflearn
pip install pillow
pip install scipy

### Install OPENCV 3.2.0 ###
brew install git cmake pkg-config jpeg libpng libtiff openexr eigen tbb
pip install opencv-python

### TENSORFLOW 1.0.1 ###
TF_URL=https://storage.googleapis.com/tensorflow/mac/cpu/tensorflow-1.0.1-py3-none-any.whl
pip install --ignore-installed --upgrade $TF_URL

pip install ipykernel
python -m ipykernel install --user --name ml --display-name "Python (ml)"

#Start notebook
jupyter notebook

#Remember to set Kernel to "Python(ml) when you open a notebook"

#I will try to update this tutorial with proper formatting soon! :)
