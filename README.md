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

You may additionally need things like numpy - use: 
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