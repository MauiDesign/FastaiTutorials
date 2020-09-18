# FastaiTutorials
 Fast AI Tutorials
 
## 1. Install Homebrew

__Homebrew is a package for macOS. Install it using the following command:__

_/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"_

You should get a following message at the end:

==> Installation successful!

## 2. Install Anaconda Python

Anaconda is the easiest way to perform Python data science and machine learning on Linux, Windows, and macOS.

__You can install it quickly using the Homebrew:__

_brew cask install anaconda_

You will be asked to enter the password of your macOS user account twice and you should see this after Python and packages are installed:

🍺  anaconda was successfully installed!

__However, theconda command is not available on your PATH so you need to add it:__

_echo 'export PATH="/usr/local/anaconda3/bin:$PATH"' >> ~/.bash_profile_

__Close your terminal and reopen it again. Verify the Conda is available by issuing:__

_conda -V_

You should see the version like conda 4.6.11.

__You need to configure Conda to work well with your shell by:__

_conda init bash_

If you use a different shell than Bash then type conda init --help to see available options. You need to reopen the terminal again to see the effects.

## 3. (Optional) Create a Conda environment

A virtual environment is a named, isolated, working copy of Python that that maintains its own files, directories, and paths so that you can work with specific versions of libraries or Python itself without affecting other Python projects. It is recommended to install fastai and its prerequisites such as PyTorch to its own environment.

__Update the Conda first:__

_conda update conda_

__Create a new environment with the name fastai:__

_conda create --name fastai python=3.7_

__Activate it:__

_conda activate fastai_

## 4. Install fastai and Jupyter Notebook

__The last step is to install fastai and Jupyter Notebook using Conda:__

_conda install -c pytorch -c fastai fastai jupyter_

__To verify that it has been installed type:__

_jupyter notebook_

## 5. Create your first notebook with fastai

Now you have everything ready to try something with fastai. For example, follow this tutorial: https://docs.fast.ai/tutorial.data.html#Vision or take the Practical Deep Learning for Coders course at https://course.fast.ai/
