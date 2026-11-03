# Support Vector Machines on Iris and Faces

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

An experimental study of SVMs with scikit-learn, covering kernels, regularization, nuisance features and dimensionality reduction.

## Results

| Task | Model | Test accuracy |
| --- | --- | --- |
| Iris, 2 classes and 2 features | Linear SVM | 0.74 |
| Iris, 2 classes and 2 features | Polynomial SVM | 0.66 |
| LFW faces, 2 people | Linear SVM | **0.96** |
| LFW faces with 300 nuisance features | Linear SVM | 0.66 |
| Same noisy data after PCA | Linear SVM | 0.76 |
| LFW faces, 2 people | RBF SVM (C = 10) | 0.95 |

Nuisance features sharply degrade the linear SVM, and PCA recovers part of the lost accuracy.

## Getting started

```bash
pip install -r requirements.txt
jupyter notebook svm_iris_face_classification.ipynb
```

Both datasets load through scikit-learn.

## Author

**Yassine Houari** · [LinkedIn](https://www.linkedin.com/in/yassine-houari-/)
