# wp-knn

This repository contains all code samples described in the [_Machine Learning in kdb+: k-Nearest Neighbor classification and pattern recognition with q_](http://code.kx.com/q/wp/machine_learning_in_kdb.pdf) whitepaper.


Code samples in `knn_digits.q` are intended to assist the user with building, testing, and benchmarking a k-NN classifier.

`knn_utils.q` is a usable kNN util library with the necessary functions and helpers to:
* calculate distance metric
* extract the k-nearest neighbors
* classify a test instance
* benchmark a classifier

To start the whitepaper demonstration, download the training and validation set mentioned in Chapter 1, and run from the same folder: 
```bash
q knn_digits.q -s x
```
To load the the k-NN library:
```bash
q knn_utils.q -s x
```
Or
```q
q)\l knn_utils.q
```
