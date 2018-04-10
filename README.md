# How to convince Inception you're a teapot.



## Installation

You need Python (3.5 or above), [Tensorflow](https://www.tensorflow.org/install/), [Keras](https://keras.io/) and cleverhans to be installed.  

Install cleverhans:
~~~
pip install -e git+https://github.com/tensorflow/cleverhans.git#egg=cleverhans
~~~

Install PIL:
~~~
pip install pillow
~~~

You may additionally need things like `numpy` - use: 
~~~
pip install <thing>
~~~
for any scientific python libraries you are missing.


## How to run

First, find an image you would like to use as an input and supply its path.  In the example we attack an unsuspecting goldfish, but you can choose anything you like:

~~~
IMAGE_PATH=<path_to_your_image>
~~~


Now we're ready to go:

~~~
$ python teapot_attack.py
~~~



## Exercises

1. Find an image of a goldfish and run the iterative attack.  What class is it classified after one iteration?

2. Try changing the parameter `eps` - what does it do?  Does it change the answer to question 1?

3. Change the attack so that it is an *untargeted* attack.  You'll need to change the arguements to the FastGradientSign method - check the documentation [here](https://cleverhans.readthedocs.io/en/latest/source/attacks.html). 

~~~
fgsm_params = {'eps': eps, 'clip_min': -1.0, 'clip_max': 1.0}
~~~

Just do this attack once don't repeat it - what might happen if you did repeat it?
