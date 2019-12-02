# CNN-Pre-Initialization-by-Minimalistic-Part-Learning-for-Handwritten-Numeral-Recognition

### Description
This paper performs handwritten numeral recognition. In this we pre-initialize the convolutional neural networks(CNN) by part learning. Two CNNs are pre-intialized with just the top-half(with bottom-half masked) and bottom-half(with top-half masked)of the 5% of the training data respectively. The CNNs are fine tuned using the remaining 95% training data. The probabilistcs softmax scores of two CNNS are fused to decide the test label.

### Usage

**Step 1. Taking 5% samples from training data.**   
Data Preparation.ipynb   
**Step 2. Preparing 5% samples for top-half view and bottom-half view**   
Top Half & Bottom Half Preparation.ipynb    
**Step 3. Pre-Intializing CNN using top-half 5% samples, fine tuning it with 95% training data and getting predicted probabilty scores.**     Fine tuning after pre-initialization (top-half part).ipynb   
**Step 4. Pre-Intializing CNN using bottom-half 5% samples, fine tuning it with 95% training data and getting predicted probabilty scores.**   
Fine tuning after pre-initialization (bottom-half part).ipynb   
**Step 5. Fusing the scores (average or max function) to predict the output class.**     
Combining Top-half and Bottom-half Predictions.ipynb   
### Citation

If using this code, please cite our work using :

	Susan, Seba, and Jatin Malhotra. "CNN Pre-Initialization by Minimalistic Part-Learning for Handwritten Numeral Recognition." In International Conference on Mining Intelligence and Knowledge Exploration. Springer, Cham, 2019.
