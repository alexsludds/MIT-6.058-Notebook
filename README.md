# MIT-6.058-Notebook
This is a notebooks collection I made for the MIT IAP Signals and Systems class
The course is taught using jupyter-notebook with a python3 kernel.
# Install Instructions

## Linux
Run the following for apt to be able to install the necessary packages inside of your terminal:

sudo apt-get install git python3 

Open the terminal and navigate to where you wish to store the files for this course. Then type:

git clone https://github.com/alexsludds/MIT-6.058-Notebook.git

If you do have it run the following command in the terminal:

sudo pip3 install --upgrade pip

We will now install all of the python packages that we will be using within the course.

Navigate gitbash to the directory with req.txt in it and type:

sudo pip3 install --upgrade -r req.txt

## Windows
If you don't already you should get a copy of python3:
https://www.python.org/downloads/

First thing you must install gitbash (http://gitforwindows.org/)

You should only have to select the first option of anything during installation.

After installing gitbash open gitbash and navigate to where you wish to store the files for this course. Then type:

git clone https://github.com/alexsludds/MIT-6.058-Notebook.git

Then we are going to make sure that you have the most recent version of pip. 

Most versions of python ship with pip these days, but somoe people may not have it. If you don't have it consult the following:
https://pip.pypa.io/en/stable/installing/#do-i-need-to-install-pip

If you do have it run the following command in gitbash:
pip3 install --upgrade pip

We will now install all of the python packages that we will be using within the course.

Navigate gitbash to the directory with req.txt in it and type:

pip3 install --upgrade -r req.txt

This may take several minutes

## Mac OS

Open the terminal and navigate to where you wish to store the files for this course. Then type:

git clone https://github.com/alexsludds/MIT-6.058-Notebook.git

If you do have it run the following command in the terminal:

sudo pip3 install --upgrade pip

We will now install all of the python packages that we will be using within the course.

Navigate gitbash to the directory with req.txt in it and type:

sudo pip3 install --upgrade -r req.txt

In addition to installing the above software on your machine in order to run the notebooks we will 
also need to tweak some of the properties so that we can play long audio etc, please do the following:

# Configure Jupyter Notebook
type in gitbash or terminal: jupyter notebook --generate-config

This will generate a configuration file in your home directory, most likely it will be ~/.jupyter/jupyter_notebook_config.py

Edit this file and locate the line that reads: c.NotebookApp.iopub_data_rate_limit

Uncomment and change the value to 10000000 (just add a zero) 

This step is important for us to play long audio clips in Jupyter Notebook (anything longer than ~1 minute) 

