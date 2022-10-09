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

&nbsp;&nbsp;&nbsp;&nbsp;**Windows**
* Go to https://www.anaconda.com/products/individual and click the “Download” button
* Download the Python 3.8 64-Bit Graphical Installer or the 32-Bit Graphical Installer installer, per your system requirements
* Run the downloaded executable (.exe) file to begin the installation. See here for more details
* (Optional) In the next step, check the box “Add Anaconda3 to my PATH environment variable”. This will make Anaconda your default Python distribution, which should ensure that you have the same default Python distribution across all editors.

&nbsp;&nbsp;&nbsp;&nbsp;**Linux**
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
* **Important-**
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
* **Important-**
  Throughout the rest of the tutorial, execution of any commands in a ***Terminal*** window should be done after the Anaconda virtual environment has been activated!

## TensorFlow Installation
Getting setup with an installation of TensorFlow can be done in 3 simple steps.
  &nbsp;&nbsp;&nbsp;&nbsp;### Install the TensorFlow PIP package
  * Run the following command in a ***Terminal*** window:
  ```bash
  pip install --ignore-installed --upgrade tensorflow==2.9.1
  ```
  &nbsp;&nbsp;&nbsp;&nbsp;### Verify your Installation
  * Run the following command in a ***Terminal*** window:
  ```bash
  python -c "import tensorflow as tf;print(tf.reduce_sum(tf.random.normal([1000, 1000])))"
  ```
  * Once the above is run, you should see a print-out similar to the one bellow:
  ```bash
  2020-06-22 19:20:32.614181: W tensorflow/stream_executor/platform/default/dso_loader.cc:55] Could not load dynamic library 'cudart64_101.dll'; dlerror:0 cudart64_101.dll not found
  2020-06-22 19:20:32.620571: I tensorflow/stream_executor/cuda/cudart_stub.cc:29] Ignore above cudart dlerror if you do not have a GPU set up on your machine.
  2020-06-22 19:20:35.027232: I tensorflow/stream_executor/platform/default/dso_loader.cc:44] Successfully opened dynamic library nvcuda.dll
  2020-06-22 19:20:35.060549: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1561] Found device 0 with properties:
  pciBusID: 0000:02:00.0 name: GeForce GTX 1070 Ti computeCapability: 6.1
  coreClock: 1.683GHz coreCount: 19 deviceMemorySize: 8.00GiB deviceMemoryBandwidth: 238.66GiB/s
  2020-06-22 19:20:35.074967: W tensorflow/stream_executor/platform/default/dso_loader.cc:55] Could not load dynamic library 'cudart64_101.dll'; dlerror: cudart64_101.dll not found
  2020-06-22 19:20:35.084458: W tensorflow/stream_executor/platform/default/dso_loader.cc:55] Could not load dynamic library 'cublas64_10.dll'; dlerror: cublas64_10.dll not found
  2020-06-22 19:20:35.094112: W tensorflow/stream_executor/platform/default/dso_loader.cc:55] Could not load dynamic library 'cufft64_10.dll'; dlerror: cufft64_10.dll not found
  2020-06-22 19:20:35.103571: W tensorflow/stream_executor/platform/default/dso_loader.cc:55] Could not load dynamic library 'curand64_10.dll'; dlerror: curand64_10.dll not found
  2020-06-22 19:20:35.113102: W tensorflow/stream_executor/platform/default/dso_loader.cc:55] Could not load dynamic library 'cusolver64_10.dll'; dlerror: cusolver64_10.dll not found
  2020-06-22 19:20:35.123242: W tensorflow/stream_executor/platform/default/dso_loader.cc:55] Could not load dynamic library 'cusparse64_10.dll'; dlerror: cusparse64_10.dll not found
  2020-06-22 19:20:35.140987: I tensorflow/stream_executor/platform/default/dso_loader.cc:44] Successfully opened dynamic library cudnn64_7.dll
  2020-06-22 19:20:35.146285: W tensorflow/core/common_runtime/gpu/gpu_device.cc:1598] Cannot dlopen some GPU libraries. Please make sure the missing libraries mentioned above are installed properly if you would like to use GPU. Follow the guide at https://www.tensorflow.org/install/gpu for how to download and setup the required libraries for your platform.
  Skipping registering GPU devices...
  2020-06-22 19:20:35.162173: I tensorflow/core/platform/cpu_feature_guard.cc:143] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
  2020-06-22 19:20:35.178588: I tensorflow/compiler/xla/service/service.cc:168] XLA service 0x15140db6390 initialized for platform Host (this does not guarantee that XLA will be used). Devices:
  2020-06-22 19:20:35.185082: I tensorflow/compiler/xla/service/service.cc:176]   StreamExecutor device (0): Host, Default Version
  2020-06-22 19:20:35.191117: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1102] Device interconnect StreamExecutor with strength 1 edge matrix:
  2020-06-22 19:20:35.196815: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1108]
  tf.Tensor(1620.5817, shape=(), dtype=float32)
  ```
## GPU Support (Optional)
  Although using a GPU to run TensorFlow is not necessary, the computational gains are substantial. Therefore, if your machine is equipped with a compatible CUDA-enabled GPU, it is recommended that you follow the steps listed below to install the relevant libraries necessary to enable TensorFlow to make use of your GPU.

By default, when TensorFlow is run it will attempt to register compatible GPU devices. If this fails, TensorFlow will resort to running on the platform’s CPU. This can also be observed in the printout shown in the previous section, under the “Verify the install” bullet-point, where there are a number of messages which report missing library files (e.g. ` Could not load dynamic library 'cudart64_101.dll'; dlerror: cudart64_101.dll not found `)

In order for TensorFlow to run on your GPU, the following requirements must be met:
**Prerequisites**
* Nvidia GPU (GTX 650 or newer)
* CUDA Toolkit v11.3.1
* CuDNN 8.2.1

&nbsp;&nbsp;&nbsp;&nbsp;### Install CUDA Toolkit & CUDNN
```bash
conda install -c anaconda cudatoolkit
```
## Environment Setup
  &nbsp;&nbsp;&nbsp;&nbsp;### Windows
  * Go to Start and Search “environment variables”
  * Click “Edit the system environment variables”. This should open the “System Properties” window
  * In the opened window, click the “Environment Variables…” button to open the “Environment Variables” window.
  * Under “System variables”, search for and click on the `Path` system variable, then click “Edit…”
  * Add the following paths, then click “OK” to save the changes:
    
    * `<INSTALL_PATH>\NVIDIA GPU Computing Toolkit\CUDA\v11.2\bin`
    * `<INSTALL_PATH>\NVIDIA GPU Computing Toolkit\CUDA\v11.2\libnvvp`
    * `<INSTALL_PATH>\NVIDIA GPU Computing Toolkit\CUDA\v11.2\include`
    * `<INSTALL_PATH>\NVIDIA GPU Computing Toolkit\CUDA\v11.2\extras\CUPTI\lib64`
    * `<INSTALL_PATH>\NVIDIA GPU Computing Toolkit\CUDA\v11.2\cuda\bin`

  &nbsp;&nbsp;&nbsp;&nbsp;### Linux
  * As per Section 7.1.1 of the [CUDA Installation Guide for Linux](https://docs.nvidia.com/deeplearning/sdk/cudnn-install/index.html#install-linux), append the following lines to `~/.bashrc` :
  ```bash
  # CUDA related exports
export PATH=/usr/local/cuda-11.2/bin${PATH:+:${PATH}}
export LD_LIBRARY_PATH=/usr/local/cuda-11.2/lib64${LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}
  ```
  
## Verify the installation
* Run the following command in a **NEW** *Terminal* window:
```python
  python -c "import tensorflow as tf;print(tf.reduce_sum(tf.random.normal([1000, 1000])))"
```
* **Important-** A new terminal window must be opened for the changes to the Environmental variables to take effect!!
* Once the above is run, you should see a print-out similar to the one bellow:
```bash
2021-06-08 18:28:38.452128: I tensorflow/stream_executor/platform/default/dso_loader.cc:53] Successfully opened dynamic library cudart64_110.dll
2021-06-08 18:28:40.948968: I tensorflow/stream_executor/platform/default/dso_loader.cc:53] Successfully opened dynamic library nvcuda.dll
2021-06-08 18:28:40.973992: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1733] Found device 0 with properties:
pciBusID: 0000:02:00.0 name: GeForce GTX 1070 Ti computeCapability: 6.1
coreClock: 1.683GHz coreCount: 19 deviceMemorySize: 8.00GiB deviceMemoryBandwidth: 238.66GiB/s
2021-06-08 18:28:40.974115: I tensorflow/stream_executor/platform/default/dso_loader.cc:53] Successfully opened dynamic library cudart64_110.dll
2021-06-08 18:28:40.982483: I tensorflow/stream_executor/platform/default/dso_loader.cc:53] Successfully opened dynamic library cublas64_11.dll
2021-06-08 18:28:40.982588: I tensorflow/stream_executor/platform/default/dso_loader.cc:53] Successfully opened dynamic library cublasLt64_11.dll
2021-06-08 18:28:40.986795: I tensorflow/stream_executor/platform/default/dso_loader.cc:53] Successfully opened dynamic library cufft64_10.dll
2021-06-08 18:28:40.988451: I tensorflow/stream_executor/platform/default/dso_loader.cc:53] Successfully opened dynamic library curand64_10.dll
2021-06-08 18:28:40.994115: I tensorflow/stream_executor/platform/default/dso_loader.cc:53] Successfully opened dynamic library cusolver64_11.dll
2021-06-08 18:28:40.998408: I tensorflow/stream_executor/platform/default/dso_loader.cc:53] Successfully opened dynamic library cusparse64_11.dll
2021-06-08 18:28:41.000573: I tensorflow/stream_executor/platform/default/dso_loader.cc:53] Successfully opened dynamic library cudnn64_8.dll
2021-06-08 18:28:41.001094: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1871] Adding visible gpu devices: 0
2021-06-08 18:28:41.001651: I tensorflow/core/platform/cpu_feature_guard.cc:142] This TensorFlow binary is optimized with oneAPI Deep Neural Network Library (oneDNN) to use the following CPU instructions in performance-critical operations:  AVX AVX2
To enable them in other operations, rebuild TensorFlow with the appropriate compiler flags.
2021-06-08 18:28:41.003095: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1733] Found device 0 with properties:
pciBusID: 0000:02:00.0 name: GeForce GTX 1070 Ti computeCapability: 6.1
coreClock: 1.683GHz coreCount: 19 deviceMemorySize: 8.00GiB deviceMemoryBandwidth: 238.66GiB/s
2021-06-08 18:28:41.003244: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1871] Adding visible gpu devices: 0
2021-06-08 18:28:42.072538: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1258] Device interconnect StreamExecutor with strength 1 edge matrix:
2021-06-08 18:28:42.072630: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1264]      0
2021-06-08 18:28:42.072886: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1277] 0:   N
2021-06-08 18:28:42.075566: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1418] Created TensorFlow device (/job:localhost/replica:0/task:0/device:GPU:0 with 6613 MB memory) -> physical GPU (device: 0, name: GeForce GTX 1070 Ti, pci bus id: 0000:02:00.0, compute capability: 6.1)
```
* Notice from the lines highlighted above that the library files are now `Successfully opened` and a debugging message is presented to confirm that TensorFlow has successfully `Created TensorFlow device`.
  
## TensorFlow Object Detection API Installation
Now that you have installed TensorFlow, it is time to install the TensorFlow Object Detection API.
&nbsp;&nbsp;&nbsp;&nbsp;### Downloading the TensorFlow Model Garden
* Create a new folder under a path of your choice and name it `TensorFlow`. (e.g.`C:\Users\sglvladi\Documents\TensorFlow`).
 
  
  
#<p align="center">
#<img src="https://user-images.githubusercontent.com/89768465/194772094-c56c292f-c245-47c1-8d46-9b4c9305afb0.gif">
#</p>
#<p align="center">
#<img src="https://user-images.githubusercontent.com/89768465/194772007-948fac47-29b7-45e9-906f-61e4201c2f99.gif">
#</p>
