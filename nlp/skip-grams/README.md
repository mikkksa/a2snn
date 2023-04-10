## Method
We take simple [N-Gram model](https://pytorch.org/tutorials/beginner/nlp/word_embeddings_tutorial.html). Slightly changing it adding some usual info such as batch accuracy calculation. Then we take simple [SNN](https://snntorch.readthedocs.io/en/latest/tutorials/tutorial_6.html) and modify it to process the same task unifying these models in some aspects.

## Results
**For M1 processor**

| Metric | ANN | SNN |
| ----- | ------ | ------ |
| Epochs | 10 | 20 |
| Accuracy, % | 100 | ~85 |
| 100% Epoch | 3 | inf |
| Time, seconds | 0.55 | 61 |

### Conclusion
Without using special hardware for SNNs, ANNs have a huge outperform on very small texts for all metrics. It is interesting to check that on different datasets
