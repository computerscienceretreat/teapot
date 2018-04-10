# teapot
Adversarial examples with keras and cleverhans


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


## How to 

First

~~~
IMAGE_PATH=<path_to_your_image>
~~~