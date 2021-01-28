# FOIT: Fast Online Instance Transfer for Improved EEG Emotion Recognition

The Electroencephalogram (EEG)-based emotion recognition is promising yet limited by the requirement of large number of training samples. Collecting substantial labeled samples in the training trails is the key to good classification performance on the test trails. This process is time-consuming and laborious. In recent years, several studies have proposed various semi-supervised learning (e.g., active learning) and transfer learning (e.g., domain adaptation, style transfer mapping) methods to reduce the requirement on training data. However, most of them are iterative methods, which need considerable training time and are unfeasible in practice. To tackle this problem, we present the Fast Online Instance Transfer (FOIT) for improved EEG emotion recognition. FOIT selects auxiliary data from historical sessions or other subjects with high confidence on prediction of the baseline model, which are then combined with the training data for classifier training. The predictions on the test trails are made by the ensemble classifier. FOIT is a one-shot method, which avoids the time-consuming iterations. Experimental results demonstrate that FOIT brings significant accuracy improvement for the three-category classification (1%-8%) on the SEED dataset and four-category classification (1%-14%) on the SEED-IV dataset in three transfer situations. The time cost for our machine over the baselines is moderate (~25s in average on two datasets in three transfer situations). To achieve the comparative accuracies, the iterative methods require much more time (~30s - ~1400s). FOIT provides a practically feasible solution to improve the generalization of emotion recognition models and allows various choices of classifiers without any constrains.

## Usage

Run `python FOIT_ultra.py`, and the results will be printed in the terminal.

## Contributing
Issues are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
