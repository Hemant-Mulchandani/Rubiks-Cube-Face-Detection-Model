# [🧮Rubik's Cube Face Detection Model🚦](https://github.com/Hemant-Mulchandani/Rubiks-Cube-Face-Detection-Model)

<p align="center">
  <img src="https://user-images.githubusercontent.com/89768465/194771951-de426a39-4a8e-46e9-a167-9c3bd672f39b.gif">
</p>

# Installation :package:
* **General Remarks**
In contrast to TensorFlow 1.x, where different Python packages needed to be installed for one to run TensorFlow on either their CPU or GPU (namely `  tensorflow ` and `  tensorflow-gpu `), TensorFlow 2.x only requires that the `  tensorflow ` package is installed and automatically checks to see if a GPU can be successfully registered.

## Anaconda Python 3.8 (Optional)
Although having Anaconda is not a requirement in order to install and use TensorFlow, I suggest doing so, due to it’s intuitive way of managing packages and setting up new virtual environments. Anaconda is a pretty useful tool, not only for working with TensorFlow, but in general for anyone working in Python, so if you haven’t had a chance to work with it, now is a good chance.

## Install Anaconda Python 3.8
**Windows**
* Go to https://www.anaconda.com/products/individual and click the “Download” button
* Download the Python 3.8 64-Bit Graphical Installer or the 32-Bit Graphical Installer installer, per your system requirements
* Run the downloaded executable (.exe) file to begin the installation. See here for more details
* (Optional) In the next step, check the box “Add Anaconda3 to my PATH environment variable”. This will make Anaconda your default Python distribution, which should ensure that you have the same default Python distribution across all editors.

**Linux**
* Go to https://www.anaconda.com/products/individual and click the “Download” button
* Download the Python 3.8 64-Bit (x86) Installer
* Run the downloaded bash script (.sh) file to begin the installation. See here for more details.
* When prompted with the question “Do you wish the installer to prepend the Anaconda<2 or 3> install location to PATH in your /home/<user>/.bashrc ?”, answer “Yes”. If you enter “No”, you must manually add the path to Anaconda or conda will not work.

## Create a new Anaconda virtual environment
* Open a new Terminal window
* Type the following command:
  ```bash
  conda create -n tensorflow pip python=3.7
  ```
* The above will create a new virtual environment with name tensorflow
* **Important**
  The term Terminal will be used to refer to the ***Terminal*** of your choice (e.g. Command Prompt, Powershell, etc.)

## Activate the Anaconda virtual environment
* Activating the newly created virtual environment is achieved by running the following in the ***Terminal*** window:
  ```bash
  conda activate tensorflow
  ```
* Once you have activated your virtual environment, the name of the environment should be displayed within brackets at the beggining of your cmd path specifier, e.g.:
  ```bash
  (tensorflow) C:\Users\sglvladi>
  ```
* **Important**
  Throughout the rest of the tutorial, execution of any commands in a ***Terminal*** window should be done after the Anaconda virtual environment has been activated!


<p align="center">
<img src="https://user-images.githubusercontent.com/89768465/194772094-c56c292f-c245-47c1-8d46-9b4c9305afb0.gif">
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/89768465/194772007-948fac47-29b7-45e9-906f-61e4201c2f99.gif">
</p>
