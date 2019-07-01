# ``Experimental Study of Machine-Learning-Based Detection and Identification of Physical-Layer Attacks in Optical Networks``
Carlos Natalino, Marco Schiano, Andrea Di Giglio, Lena Wosinska and Marija Furdek

**Abstract:** Optical networks are critical infrastructure supporting vital services and are vulnerable to different types of malicious attacks targeting service disruption at the optical layer. Due to the various attack techniques causing diverse physical- layer effects, as well as the limitations and sparse placement of optical performance monitoring devices, such attacks are difficult to detect, and their signatures are unknown. This paper presents a Machine Learning (ML) framework for detection and identification of physical-layer attacks, based on experimental attack traces from an operator field-deployed testbed with coherent receivers. We perform in-band and out-of-band jamming signal insertion attacks, as well as polarization modulation attacks, each with varying intensities. We then evaluate 8 different ML classifiers in terms of their accuracy, and scalability in processing experimental data. The optical parameters critical for accurate attack identification are identified and the generalization of the models is validated. Results indicate that Artificial Neural Networks (ANNs) achieve 99.9% accuracy in attack type and intensity classification, and are capable of processing 1 million samples in less than 10 seconds.

Paper available at <a href="https://ieeexplore.ieee.org/document/8738965" target="_blank">IEEE Xplore</a>.

## The code will be shared here once the paper is published online.

## What is in this repo?
We are releasing the following:
* Implementation of the machine learning models presented in the paper
* Analysis of the dataset *(dataset is not available due to confidentiality restrictions)*
* Trained models (inside `models` folder)
* Generated plots (inside `figures` folder)

## Setting up your environment (which libraries are required?)

You can setup you environment using Python 3.6 or Python 3.7:

**Python 3.6**: The `time.time_ns()` (which returns current time in nanoseconds) function should be replaced by `time.time()` (which returns current time in miliseconds)

In the command line, at the folder containing this repository, you can run:

**If you are running Anaconda:** 

`conda env create -f venv37-tf13-cpu.yml.yml` 

or 

`conda create --name <env_name> --file requirements.txt`.

**If you are running pip:** 

`pip install --user --requirement requirements.txt`.

### Citing the work

Bibtex entry:

~~~~
@ARTICLE{NatalinoEtAl:2019:JLT, 
    author={C. {Natalino} and M. {Schiano} and A. {Di Giglio} and L. {Wosinska} and M. {Furdek}}, 
    journal={Journal of Lightwave Technology}, 
    title={Experimental Study of Machine-Learning-Based Detection and Identification of Physical-Layer Attacks in Optical Networks}, 
    year={2019}, 
    doi={10.1109/JLT.2019.2923558}
    }
~~~~

## References and tutorials useful during the development of this work:

* Multi-Class Classification Tutorial with the Keras Deep Learning Library (https://machinelearningmastery.com/multi-class-classification-tutorial-keras-deep-learning-library/)
* Train/Test Split and Cross Validation in Python (https://towardsdatascience.com/train-test-split-and-cross-validation-in-python-80b61beca4b6)
* Use Keras Deep Learning Models with Scikit-Learn in Python (https://machinelearningmastery.com/use-keras-deep-learning-models-scikit-learn-python/)