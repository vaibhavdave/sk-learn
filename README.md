# sk-learn

A structured, hands-on syllabus for learning machine learning: **theory
first, then implementation and evaluation**, inside Jupyter notebooks with
visualizations to build intuition. Modules 00-09 cover classic ML with
scikit-learn; modules 10+ continue into deep learning with PyTorch (and a
TensorFlow/Keras comparison module).

## How each notebook is organized

1. **Theory** — intuition, core math/formula, assumptions, pros/cons, when to use it
2. **Implementation** — the algorithm applied to a real or synthetic dataset via sklearn
3. **Evaluation** — relevant metrics and diagnostic plots
4. **Exercises** — small variations to reinforce the concept

## Setup

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

## Syllabus

| Module | Topic |
|---|---|
| [00_foundations](00_foundations) | ML types, bias-variance tradeoff, overfitting/underfitting, train/test split & cross-validation concepts |
| [01_data_preprocessing](01_data_preprocessing) | Missing values, encoding, scaling, CV strategies, regression & classification evaluation metrics |
| [02_regression](02_regression) | Linear, Ridge/Lasso/ElasticNet, Polynomial, Decision Tree, Random Forest, Gradient Boosting, SVR |
| [03_classification](03_classification) | Logistic Regression, KNN, Naive Bayes, Decision Trees, SVM, Random Forest |
| [04_ensemble_methods](04_ensemble_methods) | Bagging, AdaBoost, Gradient Boosting, Voting, Stacking |
| [05_unsupervised_learning](05_unsupervised_learning) | K-Means, Hierarchical Clustering, DBSCAN, PCA, t-SNE, Anomaly Detection |
| [06_model_selection_tuning](06_model_selection_tuning) | Pipelines, GridSearchCV/RandomizedSearchCV, learning & validation curves |
| [07_imbalanced_and_feature_selection](07_imbalanced_and_feature_selection) | Class weights, SMOTE, feature importance, RFE, SelectKBest |
| [08_neural_nets_intro](08_neural_nets_intro) | sklearn's MLPClassifier/MLPRegressor (bridge topic, not full deep learning) |
| [09_capstone_project](09_capstone_project) | End-to-end project applying the full pipeline to a real dataset |
| [10_deep_learning_foundations](10_deep_learning_foundations) | PyTorch tensors, autograd/computation graphs, verifying gradients by hand, a raw-tensor forward pass |
| [11_pytorch_training](11_pytorch_training) | `nn.Module`, MSE vs. Cross-Entropy loss, SGD/Momentum/Adam comparison, full `DataLoader` training loop, vs. sklearn's MLPClassifier |
| [12_training_deep_networks](12_training_deep_networks) | Weight initialization, Dropout, weight decay, BatchNorm, learning rate scheduling, early stopping |
| [13_tensorflow_keras](13_tensorflow_keras) | Same tensors/autograd/MLP/training-loop concepts rebuilt in TensorFlow/Keras, directly compared against modules 10-11 |
| [14_cnn_fundamentals](14_cnn_fundamentals) | Convolution & pooling from first principles, building/training a small CNN, visualizing learned filters and feature maps, vs. Module 11's MLP |
| [15_deeper_cnns_transfer_learning](15_deeper_cnns_transfer_learning) | BatchNorm in CNNs, skip connections (ResNet idea), data augmentation, and a self-contained transfer learning demo on FashionMNIST |
| [16_rnns_lstms_grus](16_rnns_lstms_grus) | RNN recurrence & sine-wave forecasting, vanishing gradients demonstrated on a long-range dependency task, LSTM/GRU gating, hidden state visualization |

Datasets used are small, well-known sklearn built-ins (iris, wine, breast
cancer, diabetes, digits) or synthetic (`make_classification`, `make_regression`,
`make_blobs`, `make_moons`) so every notebook runs quickly with no external
downloads.

### Deep learning track (10+)

Continues the same theory -> implementation -> evaluation structure, using
PyTorch as the primary framework (with a dedicated module comparing against
TensorFlow/Keras). Planned: PyTorch foundations & training practice, a
TensorFlow/Keras equivalence module, CNNs & transfer learning, RNNs/LSTMs,
Transformers, autoencoders, and a deep learning capstone.
