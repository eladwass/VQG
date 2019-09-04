# Visual Question Generating
This project task is to ask a natural and engaging question when shown an image inspired by the article Generating Natural Questions About an Image

# Results
You can look at those examples to feel the results:

![1st example](https://github.com/eladwass/VQG/blob/master/result/party.png?raw=true)

![2nd example](https://github.com/eladwass/VQG/blob/master/result/store.png?raw=true)

# Explanation of Jupyter Notebooks:
```Download datasets.ipynb```
A Jupyter Notebook that downloads images and questions from the dataset link 
<a href='https://www.microsoft.com/en-us/download/details.aspx?id=53670'>here</a>
The dataset is orgenised by the source of the image: Bing, MSCOCO, or Flickr, then by type of dataset: train, dev and test.
This notebook is mainly inspired by this repo
 <a href="https://github.com/gitlost-murali/Natural-Questions-Generation-from-Images">here</a>.
 After fully running this Notebook you can procceed to the next notebook ```VGQ-PyTorch.ipynb``` to train and see some results

```VQG-PyTorch.ipynb```
This Jupyter Notebook can run in 2 mode: train, predict.
Feel free to change the ```to_train``` variable in the second cell to False if you no longer need to train.

This notebook has mainely three parts:
1. Building the train, validation, test set by encoding the images and join them with the question
2. Training the GRNN with multiple variables
3. Predict and show the results using beam search


# References

[1] Nasrin Mostafazadeh, Ishan Misra, Jacob Devlin, Margaret Mitchell, Xiaodong He and Lucy Vanderwende<a href="https://arxiv.org/pdf/1603.06059.pdf">Generating Natural Questions About an Image</a>

