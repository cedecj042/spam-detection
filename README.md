# Spam Detection using Naive Bayes Classifier

A programming assignment for AI201 using naive bayes classifier to detect spam or ham among the emails. The dataset used in trainig was TREC06 Corpus which is a popular dataset for spam detection algorithms.

## Training and Test Set
In order to load the test and training dataset used which is uploaded in huggingface, install datasets in hugging face.

```
pip install datasets
```

Then, use the following Python code in your notebook to load the train and test splits:
```python
from datasets import load_dataset

# Load the full dataset, which returns a DatasetDict object
dataset = load_dataset("lepuer/naive-bayes")

# Access the individual splits
train_set = dataset['train']
test_set = dataset['test']

# You can now print the number of examples in each split
print(f"Training examples: {len(train_set)}")
print(f"Test examples: {len(test_set)}")

# Inspect the first example of the training set
print("\nFirst training example:")
print(train_set[0])
```
