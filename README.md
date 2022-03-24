# EPIC-KITCHENS Multi-Instance Retrieval (MIR) baselines

Train/Test splits for the Multi-Instance Retrieval Challenge are available [here](https://github.com/epic-kitchens/epic-kitchens-100-annotations/tree/master/retrieval_annotations)

To participate and submit results to the challenge, refer to the [Multi-Instance Retrieval Codalab Challenge](https://codalab.lisn.upsaclay.fr/competitions/617)

Full information about how to use the jPoSE code can be found [here](https://github.com/mwray/Joint-Part-of-Speech-Embeddings).

Full information about how to use the MI-MM code can be found [here](https://github.com/adrianofragomeni/MI-MM).

## Trained Models

Trained models can be found within `data/models` for both MLP and JPoSE by downloading the data folder [here](https://www.dropbox.com/s/bs6y50xkl1rbe20/JPoSE_data.zip?dl=0).
These were trained using PyTorch with the arguments within the `args.txt` files.

Trained models can be found within `data/models` for MI-MM by downloading the data folder [here](https://www.dropbox.com/home/MI-MM).

## Video Features

Features extracted using TBN[1] can be found at on dropbox separated for [train](https://www.dropbox.com/s/41pgqys8e9i2rjh/features_train.pkl?dl=0) and [test](https://www.dropbox.com/s/1kereto93y09ecz/features_test.pkl?dl=0) (~10GB). Both are pickle files containing the features for the Multi-Instance Retrieval train and test splits respectively.

Each represents a python dictionary containing the 'RGB', 'Flow' and 'Audio' features as a matrix of size nx25x1024 where n is the number of videos (67,217/9,668). The ordering of the videos is the same as in EPIC_100_retrieval_train.pkl and EPIC_100_retrieval_test.pkl found in the EPIC-KITCHENS-100 repo.

Temporally grouped features (mean/max) can be found in the data folder [here](https://www.dropbox.com/s/bs6y50xkl1rbe20/JPoSE_data.zip?dl=0).

Features extracted using S3D trained on HowTo100M can be found within `data/features` by downloading the data folder [here](https://www.dropbox.com/home/MI-MM).

## Training and Evaluation

Information for training and evaluating models can be found in the [JPoSE repo](https://github.com/mwray/Joint-Part-of-Speech-Embeddings) and [MI-MM repo](https://github.com/adrianofragomeni/MI-MM), including how to generate a submission file for the codalab challenge.


