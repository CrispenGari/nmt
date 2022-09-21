### Neural Machine Translation (nmt) and Language Identification (li).

🎗 This repository contains an end-to-end deep artificial neural network for machine translation and language identification based on south-african-languages.

<p align="center">
    <img src="/images/logo.png" width="50%" alt="logo"/>
</p>

### Notebooks

All the notebooks that were used in this project are found in the `notebooks` folder. Here is the folder structure:

```shell
notebooks:
        ├───bi-nmt
        ├───lang-identification
        │   ├───datasets
        │   └───model
        ├───languages
        └───nmt-gathering
```

### Language Identification

In this model we created a language identification model that identifies `6` south african languages. These languages are as follows:

```

```

The model was able to perform very well during inference and we evaluated with the following metrics on the test examples.

1. confusion matrix

<img src="/images/cm.png" alt="cm" width="100%"/>

2. classification report

```shell
                precision    recall  f1-score   support

          af       1.00      0.99      0.99      4542
          ts       1.00      0.98      0.99      4604
          st       0.98      0.99      0.98      4462
          en       0.96      1.00      0.98      4692
          xh       0.98      0.97      0.98      4571
          zu       0.98      0.97      0.98      4651

    accuracy                           0.98     27522
   macro avg       0.98      0.98      0.98     27522
weighted avg       0.98      0.98      0.98     27522
```

3. loss

The model was trained and be able to have a loss reduced to `0.058` on test examples.

4. accuracy

The model was trained and be able to obtain an accuracy of `98.35% ` on test examples.

### License

In this repository I'm using the `MIT` License which reads as follows:

```
MIT License

Copyright (c) 2022 crispengari

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

```
