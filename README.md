# machine_learning
## Prerequisites 
1. Tensor flow back end
2. HDF5 and h5py
3. Keras
### Install Tensor flow:
1. Install pip and virtualenv by issuing the following commands:
```
$ sudo easy_install pip 
$ sudo pip install --upgrade virtualenv 
```

2. Create a virtualenv environment:
```
$ virtualenv --system-site-packages ~/tensorflow
```

3. Activate the virtualenv environment:
```
$ source ~/tensorflow/bin/activate
```
which will change your prompt to the following:
```
(tensorflow)$ 
```

4. Ensure pip ≥8.1 is installed:
```
(tensorflow)$ easy_install -U pip
```

5. Install TensorFlow + all required packages  into the active Virtualenv environment:
```
(tensorflow)$ pip install --upgrade tensorflow
```

6. Verify Install from within a tensor flow prepared environment e.g. (tensorflow)$
  
    1. Invoke python
    ```
    (tensorflow)$ python
    ```

    2. run the below script
    ```
    import tensorflow as tf
    hello = tf.constant('Hello, TensorFlow!')
    sess = tf.Session()
    print(sess.run(hello))
    ```
    
#### Stuff the Remember
- To Activate:
```
$ source ~/tensorflow/bin/activate
```
- To deactivate: 
```
(tensorflow)$ deactivate
```
- To uninstall:
```
$ rm -r ~/tensorflow 
```
- More Help https://www.tensorflow.org/install/


### Install HDF5
```
$ brew tap homebrew/science
$ brew install homebrew/science/hdf5
```

### Install h5py
```
$ sudo pip install --no-binary=h5py h5py
```
- invoke python and test with:
``` 
import h5py
h5py.run_tests()
```


### Install Keras
1. Activate TensorFlow: 
```
$ source ~/tensorflow/bin/activate
```
2. run:
```
$ pip install keras
```
3. test with:
```
$ curl -sSL https://github.com/fchollet/keras/raw/master/examples/mnist_mlp.py | python
```
