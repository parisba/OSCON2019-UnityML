# Tutorial Preparation

This document outlines everything you need to do before the tutorial at OSCON 2019.

## Installing Unity ML for macOS and Linux

⚠️ You'll need to have git installed, and exploring how to install git is beyond the scope of this post; so if you haven't got git installed, go do that first, then come back here!

### First, clone the ML-Agents project
First, you'll need to clone the repository for Unity ML . You can find the repository on GitHub at https://github.com/Unity-Technologies/ml-agents/

### Second, install Python 3.6
Right now, the Unity ML toolkit requires Python 3.6. Any version of Python 3.6 is suitable, but I recommend the latest release in the Python 3.6 series, Python 3.6.8.

⚠️ Unity ML requires Python 3.6 because of a long chain of reasons that mostly boil down to… the version of TensorFlow that Unity ML is currently dependent on requires Python 3.6. This will probably change in the future!

You can find installers for Python 3.6.8 on the Python website, so while you could install it using one of many package managers, in my experience simply installing the right version directly for your platform is the easiest way to do it.

⚠️ Unity ML requires Python 3.6 because of a long chain of reasons that mostly boil down to… the version of TensorFlow that Unity ML is currently dependent on requires Python 3.6. This will probably change in the future!

You can find installers for Python 3.6.8 on the Python website, so while you could install it using one of many package managers, in my experience simply installing the right version directly for your platform is the easiest way to do it.

For example, I use macOS most of the time, and on that platform I download the 'macOS 64-bit installer', which is an ordinary macOS package file that providers an installer interface.

You can verify that you've got a version of Python 3.6 installed by running the following command in your terminal:
`python --version`

If you can't find this command, or this command, try the following:
`python3.6 --version`

Either way, in response to this command you should see:
`Python 3.6.8`

If you don't see a version of Python 3.6.8, please check one of the many guides on how to install Python. 

### Third, install the Unity ML package

Once you've got the correct version of Python up and running, you'll need to use pip (pip3, to be precise) to install the mlagents package. Run the following command to do this:
`pip3 install mlagents`

You may be wondering at this point why we went to the trouble of cloning the repository for Unity ML, when all we were going to do later one was install the package from pip (Python's package manager)… well, we did this for a few reasons, but primarily because the Unity ML repository comes with the contents of the UnitySDK folder. 

The UnitySDK folder contains the example and template Unity projects, which form the starting point for your work with Unity ML. The rest of the folders in the repository contain the source for the mlagents package, which is interesting but out of the scope of this article.

To confirm that everything up until this point is correctly installed, execute the following command:
`mlagents-learn --help`

In response, you should see an ASCII art version of the Unity logo, follow by some command guidelines. If you don't see this, trace back through the earlier steps and see if you missed something.

### Finally, install Unity 2019.1
The easiest way to install and manage Unity, in my opinion, is to use the Unity Hub. You can download the Unity Hub from Unity's website: https://unity3d.com/get-unity/download 

Once you've got the Unity Hub downloaded and installed, use it to install the latest version of Unity 2019.1. At the time of writing, and as shown in the below screenshot, that's Unity 2019.1.1f1.