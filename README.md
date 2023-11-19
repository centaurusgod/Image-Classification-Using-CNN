# Image-Classification-Using-CNN
This is an example of image classification done using convolution neural network. Note that this works only for binary image classification and one needs to modify the code to make it work for classification of multiple classes. 
Install the NVIDIA GPU driver for your device from the link: https://www.nvidia.com/Download/index.aspx

NVIDIA GPU Driver Installation
Install the latest NVIDIA GPU driver for your device from NVIDIA's official website.
Version & OS Details
OS: Windows 11
Graphics Card: Nvidia GTX 1650 4GB vRAM
CUDA Version: 11.8
Download Link: CUDA 11.8
cuDNN Version: 8.7
Download Link: cuDNN Archive
TensorFlow Version: 2.5
NumPy Version: 1.19.5
Resolve zlib.dll Error
To resolve the zlib.dll error, follow these steps:

Navigate to C:\Program Files\NVIDIA Corporation\Nsight Systems 2022.4.2\host-windows-x64 and locate zlib.dll. Copy the file.

Go to C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.8\bin and paste the copied file. Rename it from zlib.dll to zlibwapi.dll.

Anaconda Environment Setup with TensorFlow
To set up an Anaconda environment with TensorFlow, follow these steps:

Create a new environment named 'tensorflow-gpu' with Python version 3.8:

bash
Copy code
conda create --name tensorflow-gpu python=3.8
Activate the environment:

bash
Copy code
conda activate tensorflow-gpu
Install TensorFlow version 2.5:

bash
Copy code
pip install tensorflow==2.5
Enable notebook support in the environment:

bash
Copy code
conda install -y -c conda-forge nb_conda
Add the environment to Jupyter Kernel:

bash
Copy code
python -m ipykernel install --user --name tensorflow-gpu --display-name "Python 3.8 (tensorflow-gpu)"
Usage in Jupyter Notebook
After opening Jupyter Notebook, change the kernel from Python to Python 3.8 (tensorflow-gpu) to leverage the TensorFlow environment.
