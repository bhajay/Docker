# Docker - Python
Python is one of the very commonly used languages in our machine learning work. This folder contains:
- Dockerfile
- runPython.sh
- requirements.txt

## Dockerfile
This is the docker file used to create the images. The files have been provided to enhance trust and transparency in our images. We are happy to add more packages, upon request.

## requirements.txt
This file contains all the python modules that have been installed and the version numbers.

## Run the image
A run script has been provided to help easily start the image. More instructions have been provided below for different OS. The images have been compiled as a multi-platform image and docker desktop will automatically pull the image appropriate to your platform.

- You can use jupyter notebook by using the command `run-jupyter`
- You can use python using the command `python`

### MacOS / Linux
- Install docker desktop (https://www.docker.com/products/docker-desktop).
- Start the desktop client.
- Open the terminal and navigate to the folder where you have files that you will use.
- Change settings in the `runPython.sh` script. Primary fields include:
  - `localfolder=${PWD}`: It will connect the current local folder so that the files in this folder and any sub-folders can be accessed from inside the container.
  - `version=latest`: Replace `latest` with the version of interest. If you do not change this, it will automatically pull the latest version for usage.
- Provide execution permissions using `chmod +x runPython.sh`
- Run the script file using `./runPython.sh`. This will start the container with root access inside Ubuntu.

### Windows 
Run instructions with screenshots for Windows is coming soon.

## Version history
The softwares available in each image is given below. We will keep this updated as new images are released.

### Version 1.0.8
This image uses Ubuntu 25.01 as the base OS with Python 3.13.4. Python packages installed include:
- pip (25.1.1)
- numpy (2.3.0)
- pandas (2.3.0)
- matplotlib (3.10.3)
- seaborn (0.13.2)
- scikit-learn (1.7.0)
- scipy (1.15.3)
- torch (2.7.1) (Will pull GPU version on compatible architectures)
- torchaudio (2.7.1)
- torchvision (0.22.1)

### Version 1.0.7
This image uses Ubuntu 25.01 as the base OS with Python 3.13.4. Python packages installed include:
- pip (25.1.1)
- numpy (2.3.0)
- pandas (2.3.0)
- matplotlib (3.10.3)
- seaborn (0.13.2)
- scikit-learn (1.7.0)
- scipy (1.15.3)
- torch (2.7.1+cpu) (CPU-only version)

### Version 1.0.6
This image uses Ubuntu 25.01 as the base OS with Python 3.13.4. Python packages installed include:
- pip (25.1.1)
- numpy (2.3.0)
- pandas (2.3.0)
- matplotlib (3.10.3)
- seaborn (0.13.2)
- scikit-learn (1.7.0)
- scipy (1.15.3)

### Version 1.0.4 / 1.0.5
This image uses Ubuntu 25.01 as the base OS with Python 3.13.4. Python packages installed include:
- pip (25.1.1)
- numpy (2.3.0)
- pandas (2.3.0)
- matplotlib (3.10.3)
- seaborn (0.13.2)

### Version 1.0.3
This image uses Ubuntu 25.01 as the base OS with Python 3.13.4. Python packages installed include:
- pip (25.1.1)
- numpy (2.3.0)
- pandas (2.3.0)

### Version 1.0.2
This image uses Ubuntu 25.01 as the base OS with Python 3.13.4. Python packages installed include:
- pip (25.1.1)
- numpy (2.3.0)

### Version 1.0.1
This image uses Ubuntu 22.04 as the base OS with Python 3.10.12. Python packages installed include:
- pip (22.0.2)
- setuptools (59.6.0)
- wheel (0.37.1)

### Version 1.0.0
This image uses Ubuntu (kinetic-20220602) as the base OS. Other softwares installed include:
- The issue with the alias added for commands "python" and "run-jupyter" have been fixed
- Python (v3.10.7)
- numpy
- scipy

# Authors

* Ajay B Harish

# License 

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

# Others

We are just trying out things. Lets try other things on main