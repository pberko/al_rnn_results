# al_rnn_results

*the train files structure is: first row is samples number and size of alephbet, the next rows are output. path-len, path *


non safety automata

for automaton
[blackbox.pdf](https://github.com/roiDaniela/run_time_verification/files/6971032/blackbox.pdf)

![image](https://user-images.githubusercontent.com/86918539/129101548-52abc69c-3461-4fae-a3d3-23baff6ca877.png)


| n_samples    | RNN            | Alergia     | EDSM          |train_files                                                              |
| :---         |     :---:      |       :---: |       :---:   |                                                                  ---:   |
| 100          | 100.00%        | 64.52%      |               |https://github.com/pberko/al_rnn_results/blob/main/tracesaut112_100.dat  |
| len x 5      | 97.35%         | 55.63%      |               |                                                                         |
|              | 4s             | 2s          |               |                                                                         |
| 2000         | 100.00%        | 80.65%      | 100.0%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut112_2000.dat |
| len x 5      | 100.00%        | 62.25%      | 100.0%        |                                                                         |
|              | 34.8s          | 8s          | 0.1s          |                                                                         |
| 5000         | 100.00%        | 83.87%      |               |https://github.com/pberko/al_rnn_results/blob/main/tracesaut112_5000.dat |
| len x 5      | 100.00%        | 60.26%      |               |                                                                         |
|              | 1.4m           | 18s         |               |                                                                         |

https://github.com/pberko/al_rnn_results/blob/main/tracesaut112_100.dat.ff.final.dot.pdf

https://github.com/pberko/al_rnn_results/blob/main/tracesaut112_2000.dat.ff.final.dot.pdf

HEATMAP for rnn (2000 samples)

![heatmap](https://user-images.githubusercontent.com/86918539/131121260-2ad54224-e214-4749-b5a9-2e4c3dd84743.png)


xls file: values are rnn distance (rnn Tensors euclidean distance) and x/y are states

https://docs.google.com/spreadsheets/d/14pIPymjSUhsbE9W4aEZr1oJjyDuhv8J5tOsHEhbg62w/edit?usp=sharing

when using all hidden layers:
https://docs.google.com/spreadsheets/d/1H3IQ-oGA6voaClurlHi0i3Y5fnDgNVeDVorLyVRRVEU/edit?usp=sharing

divide the paths to clusters - states with Kmeans using distances:
![image](https://user-images.githubusercontent.com/86918539/131515883-a779ebcb-88a8-4e12-a41b-0eb58b6a2f02.png)


xls file - alergia: values are path length in alergia graph

https://docs.google.com/spreadsheets/d/1fEgc9t4e5TaRPQdKh_7mMmPduvI6EpvpC28SgDLEkUY/edit?usp=sharing

------------------------------------------------------------------------------------------------------------------------------------


for automaton
[blackbox.pdf](https://github.com/roiDaniela/run_time_verification/files/6971064/blackbox.pdf)
![image](https://user-images.githubusercontent.com/86918539/129101620-9ec5180f-3807-4cd0-8fb1-16ce44d83409.png)


| n_samples    | RNN            | Alergia       | EDSM          |train_files                                                              |
| :---         |     :---:      |       :---:   |       :---:   |                                                                  ---:   |
| 100          | 68.63%         | 68.63%        |               |https://github.com/pberko/al_rnn_results/blob/main/tracesaut113_100.dat  |
| len x 5      | 68.16%         | 70.52%        |               |                                                                         |
|              | 4.35s          | 2s            |               |                                                                         |
| 2000         | 100.00%        | 76.47%        | 100.0%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut113_2000.dat |
| len x 5      | 100.00%        | 69.72%        | 100.0%        |                                                                         |
|              | 29.24s         | 4s            | 0.1s          |                                                                         |

https://github.com/pberko/al_rnn_results/blob/main/tracesaut113_100.dat.ff.final.dot.pdf

https://github.com/pberko/al_rnn_results/blob/main/tracesaut113_2000.dat.ff.final.dot.pdf

HEATMAP for rnn (2000 samples)

![heatmap](https://user-images.githubusercontent.com/86918539/131121286-f2bd2537-9e38-4ab0-a410-bf5388ce9572.png)

xls file: values are rnn distance (rnn Tensors euclidean distance) and x/y are states

https://docs.google.com/spreadsheets/d/1L5VXxH86Lpw69-I1ByWy1O-4Mf9WZBfy3aj_Q9p8cgw/edit?usp=sharing

when using all hidden layers:
https://docs.google.com/spreadsheets/d/1uNYfhshW5FqtsiLGN6iSW_8BbBt-svzk5_3-lwTfNfY/edit?usp=sharing

divide the paths to clusters - states with Kmeans using distances:
![image](https://user-images.githubusercontent.com/86918539/131516140-e0203330-43b2-4d26-ad87-50c9b73c7e13.png)


xls file - alergia: values are path length in alergia graph

https://docs.google.com/spreadsheets/d/1zXrBxi0-NmJ8mh2TuE4BqN5e1IJuXDr2Hhfm9TkTr0o/edit?usp=sharing


------------------------------------------------------------------------------------------------------------------------------------


for automaton
[blackbox.pdf](https://github.com/roiDaniela/run_time_verification/files/6971077/blackbox.pdf)
![image](https://user-images.githubusercontent.com/86918539/129101661-ded147eb-9ce5-4de9-acda-4b0c8e153222.png)

# (a+b)*abb

| n_samples    | RNN            | Alergia       | EDSM          |train_files                                                              |
| :---         |     :---:      |       :---:   |       :---:   |                                                                  ---:   |
| 100          | 64.52%         | 48.39%        |               |https://github.com/pberko/al_rnn_results/blob/main/tracesaut114_100.dat  |
| len x 5      | 60.26%         | 55.63%        |               |                                                                         |
|              | 4.68s          | 1s            |               |                                                                         |
| 2000         | 100.00%        | 80.65%        | 100.00%       |https://github.com/pberko/al_rnn_results/blob/main/tracesaut114_2000.dat |
| len x 5      | 100.00%        | 62.25%        | 100.00%       |                                                                         |
|              | 34.27s         | 7.26m         | 0.1s          |                                                                         |

https://github.com/pberko/al_rnn_results/blob/main/tracesaut114_100.dat.ff.final.dot.pdf

https://github.com/pberko/al_rnn_results/blob/main/tracesaut114_2000.dat.ff.final.dot.pdf

HEATMAP for rnn (2000 samples)

![heatmap](https://user-images.githubusercontent.com/86918539/131121329-baef715b-904f-433d-9228-b5a6cfe903ea.png)

xls file: values are rnn distance (rnn Tensors euclidean distance) and x/y are states

https://docs.google.com/spreadsheets/d/1KbJ0giggu_DuRWy3Gsva-plMp30cMoqTgwSGt6hM8Sc/edit?usp=sharing

when using all hidden layers:
https://docs.google.com/spreadsheets/d/1pc7QO67boBpQzlp93AOoQz1POZrm_3VLUU-ppwYkVLk/edit?usp=sharing

divide the paths to clusters - states with Kmeans using distances:
![image](https://user-images.githubusercontent.com/86918539/131516251-dcde18a7-c8e7-4908-898d-0c30b390d108.png)

xls file - alergia: values are path length in alergia graph

https://docs.google.com/spreadsheets/d/13ylblGndrQcNgo215Fs_UhLTlqSUPy_2OB19dOn9ul4/edit?usp=sharing


------------------------------------------------------------------------------------------------------------------------------------

for automaton
[blackbox.pdf](https://github.com/roiDaniela/run_time_verification/files/6971302/blackbox.pdf)
![image](https://user-images.githubusercontent.com/86918539/129101722-2ec7f39e-998a-4b21-b129-c68b940d8604.png)

# ??|a*|b*a|(a|b)*abb(a|b)*abb

| n_samples    | RNN            | Alergia      | EDSM       |train_files                                                              |
| :---         |     :---:      |       :---:  |       :---:   |                                                                  ---:   |
| 100          | 91.00%         | 90.00%       |               |https://github.com/pberko/al_rnn_results/blob/main/tracesaut115_100.dat  |
| len x 5      | 83.00%         | 83.00%       |               |                                                                         |
|              | 6s             | 2.35m        |               |                                                                         |
| 2000         | 100.00%        | 93.00%       | 100.00%       |https://github.com/pberko/al_rnn_results/blob/main/tracesaut115_2000.dat |
| len x 5      | 100.00%        | 84.00%       | 100.00%       |                                                                         |
|              | 1m             | 9.8h         | 0.8s          |                                                                         |


https://github.com/pberko/al_rnn_results/blob/main/tracesaut115_100.dat.ff.final.dot.pdf

https://github.com/pberko/al_rnn_results/blob/main/tracesaut115_2000.dat.ff.final.dot.pdf

HEATMAP for rnn (2000 samples)

![heatmap](https://user-images.githubusercontent.com/86918539/131121356-a732af78-4ed7-462e-8fb6-688b9dd2c0d2.png)

------------------------------------------------------------------------------------------------------------------------------------


safety automata

for automaton

[blackbox.pdf](https://github.com/roiDaniela/run_time_verification/blob/master/data/aut108/pdf/blackbox.pdf)

![image](https://user-images.githubusercontent.com/86918539/130486002-38971f9a-3e7b-4e86-927e-be8d953fca7b.png)

[specification.pdf](https://github.com/roiDaniela/run_time_verification/blob/master/data/aut108/pdf/spec.pdf)

![image](https://user-images.githubusercontent.com/86918539/130486058-771c998f-8db1-404f-9ae7-5978b230b03d.png)



| n_samples    | RNN            | Alergia       |train_files                                                              |
| :---         |     :---:      |       :---:   |                                                                  ---:   |
| 100          | 54.84%         | 63.2%         |https://github.com/pberko/al_rnn_results/blob/main/tracesaut108_100.dat  |
|              | 7s             | 37s           |                                                                         |
| 2000         | 91.29%         | 67.73%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut108_2000.dat |
|              | 22s            | 1m            |                                                                         |

HEATMAP for rnn (2000 samples)

![heatmap](https://user-images.githubusercontent.com/86918539/131121399-e0d1f12e-2fe9-46a2-a806-795ffb892e8d.png)

------------------------------------------------------------------------------------------------------------------------------------


for automaton

[blackbox.pdf](https://github.com/roiDaniela/run_time_verification/blob/master/data/aut109/pdf/blackbox.pdf)

![image](https://user-images.githubusercontent.com/86918539/130486497-0150d772-ce52-4858-90de-27108907e86e.png)

[specification.pdf](https://github.com/roiDaniela/run_time_verification/blob/master/data/aut109/pdf/spec.pdf)

![image](https://user-images.githubusercontent.com/86918539/130486463-f377b5f0-7fdd-4048-b8cb-0d218341974b.png)



| n_samples    | RNN            | Alergia       |train_files                                                              |
| :---         |     :---:      |       :---:   |                                                                  ---:   |
| 100          | 53.23%         | 65.65%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut109_100.dat  |
|              | 3s             | 1.2m          |                                                                         |
| 2000         | 97.10%         | 71.36%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut109_2000.dat |
|              | 22s            | 1m            |                                                                         |


HEATMAP for rnn (2000 samples)

![heatmap](https://user-images.githubusercontent.com/86918539/131121435-1b3d175e-24ce-42c0-8170-e38e7838f2b9.png)

------------------------------------------------------------------------------------------------------------------------------------


for automaton

[blackbox.pdf](https://github.com/roiDaniela/run_time_verification/blob/master/data/aut110/pdf/blackbox.pdf)

![image](https://user-images.githubusercontent.com/86918539/130486969-4414de09-80dd-4dbf-936e-d42048ac86a2.png)

[specification.pdf](https://github.com/roiDaniela/run_time_verification/blob/master/data/aut110/pdf/spec.pdf)

![image](https://user-images.githubusercontent.com/86918539/130487024-af44fddd-18d3-463e-903a-df38dfd50984.png)



| n_samples    | RNN            | Alergia       |train_files                                                              |
| :---         |     :---:      |       :---:   |                                                                  ---:   |
| 100          | 36.45%         | 52.19%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut110_100.dat  |
|              | 3s             | 5.4m          |                                                                         |
| 2000         | 72.90%         | 75.04%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut110_2000.dat |
|              | 23s            | 1m            |                                                                         |


HEATMAP for rnn (2000 samples)

![heatmap](https://user-images.githubusercontent.com/86918539/131121468-e8eb10dd-2db6-4a15-b78a-03306dadeb84.png)

------------------------------------------------------------------------------------------------------------------------------------

for automaton

[blackbox.pdf](https://github.com/roiDaniela/run_time_verification/blob/master/data/aut111/pdf/blackbox.pdf)

![image](https://user-images.githubusercontent.com/86918539/130487293-467c8edd-510b-4637-a8c8-ac1ab933d3fb.png)

[specification.pdf](https://github.com/roiDaniela/run_time_verification/blob/master/data/aut111/pdf/spec.pdf)

![image](https://user-images.githubusercontent.com/86918539/130487352-d145526a-b8f0-434c-8201-14364eec5706.png)



| n_samples    | RNN            | Alergia       |train_files                                                              |
| :---         |     :---:      |       :---:   |                                                                  ---:   |
| 100          | 40.65%         | 48.58%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut111_100.dat  |
|              | 4s             | 5.3m          |                                                                         |
| 2000         | 74.84%         | 77.49%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut111_2000.dat |
|              | 23s            | 16s           |                                                                         |


HEATMAP for rnn (2000 samples)

![heatmap](https://user-images.githubusercontent.com/86918539/131121502-bd806a0a-f147-4ee7-958b-21dae7fa4025.png)

------------------------------------------------------------------------------------------------------------------------------------


+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++


RNN

The nn is written in Pytorch
(ref I used https://github.com/bentrevett/pytorch-sentiment-analysis)

a. RNN is LSTM with the parameters:
        EMBEDDING_DIM = 100
        
        HIDDEN_DIM = 256
        
        OUTPUT_DIM = len(LABEL.vocab)
        
        N_LAYERS = 2
        
        BIDIRECTIONAL = True
        
        DROPOUT = 0.5
        
b. Loss function is Cross entropy loss (since it's multi class)

from pytorch doumentation:
class CrossEntropyLoss(_WeightedLoss):
    r"""This criterion combines :class:`~torch.nn.LogSoftmax` and :class:`~torch.nn.NLLLoss` in one single class.

    It is useful when training a classification problem with `C` classes.
    If provided, the optional argument :attr:`weight` should be a 1D `Tensor`
    assigning weight to each of the classes.
    This is particularly useful when you have an unbalanced training set.
    
c. accuracy function caculates the error according to the differnce between the predicted y and true y:


        def categorical_accuracy_test(preds, y):
            top_pred = preds.argmax(1, keepdim = True)
            correct = (1 - torch.abs((top_pred - y.view_as(top_pred)))/10).sum()
            acc = correct.float() / y.shape[0]
            return acc
 
d. multiclass predictiom:
  I chose to divide the train set to 10 classes : 0.0, 0.1 ... 1.0
  The nn suppose to predict the true class.

e. 
