# DeepNovo
Project: De novo Peptide Sequencing by Deep Learning.
Author: Hieu Tran, Research Fellow at University of Waterloo, Canada.
Email: nh2tran@uwaterloo.ca

DeepNovo is implemented and tested with Python 2.7 and TensorFlow r0.10. In addition, DeepNovo also uses Numpy and Cython.

Here we provide instructions for installing Python and TensorFlow on Linux Ubuntu.
    
    Step 1: Install Python 2.7, pip, and virtualenv using the following commands
    
        $ sudo apt-get install python2.7
        $ sudo apt-get install python-pip python-dev python-virtualenv
        
    You can then check the version of Python using the following command
    
        $ python --version
        
    Step 2: Install TensorFlow with virtualenv.

      Virtualenv is a virtual Python environment isolated from other Python development, incapable of interfering with or being affected by other Python programs on the same machine. 
      To start working with TensorFlow, you simply need to "activate" the virtual environment. 
      When you are done using TensorFlow, you may "deactivate" the environment.
      
      Step 2.1: Create a virtualenv environment using the following command
      
        $ virtualenv --system-site-packages ~/tensorflow

      Step 2.2: Activate the virtualenv environment using the following command
      
        $ source ~/tensorflow/bin/activate
        
      Step 2.3: Install TensorFlow using one of the following commands
      
        (tensorflow)$ pip install --upgrade tensorflow # with CPU support only
        
        (tensorflow)$ pip install --upgrade tensorflow-gpu  # with NVIDIA-GPU support
      
      Step 2.4: Deactivate the virtualenv environment using the following command
      
        (tensorflow)$ deactivate
        
    Step 3: Install Cython using the following command
        
        $ pip install Cython
        
  To use DeepNovo in the TensorFlow enviroment, you need to activate/deactivate the enviroment as mentioned earlier. Further details of DeepNovo usage are provided in the README files in each folder.
