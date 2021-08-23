# al_rnn_results

for automaton

[blackbox.pdf](https://github.com/roiDaniela/run_time_verification/blob/master/data/aut108/pdf/blackbox.pdf)

![image](https://user-images.githubusercontent.com/86918539/130485737-a0d9a3cd-b17d-4a97-81ae-0b554f7d2925.png)

[specification.pdf](https://github.com/roiDaniela/run_time_verification/blob/master/data/aut108/pdf/spec.pdf)

![image](https://user-images.githubusercontent.com/86918539/130485689-ccfb259b-7699-4944-8e5e-04c31388ce90.png)


| n_samples    | RNN            | Alergia       |train_files                                                              |
| :---         |     :---:      |       :---:   |                                                                  ---:   |
| 100          | 54.84%         | 63.2%         |https://github.com/pberko/al_rnn_results/blob/main/tracesaut108_100.dat  |
| 2000         | 91.29%         | 67.73%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut108_2000.dat |


*the train files structure is: first row is samples number and size of alephbet, the next rows are output. path-len, path *

for automaton
[blackbox.pdf](https://github.com/roiDaniela/run_time_verification/files/6971032/blackbox.pdf)

![image](https://user-images.githubusercontent.com/86918539/129101548-52abc69c-3461-4fae-a3d3-23baff6ca877.png)


| n_samples    | RNN            | Alergia       |train_files                                                              |
| :---         |     :---:      |       :---:   |                                                                  ---:   |
| 100          | 100.00%        | 64.52%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut112_100.dat  |
| 2000         | 100.00%        | 80.65%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut112_2000.dat |


for automaton
[blackbox.pdf](https://github.com/roiDaniela/run_time_verification/files/6971064/blackbox.pdf)
![image](https://user-images.githubusercontent.com/86918539/129101620-9ec5180f-3807-4cd0-8fb1-16ce44d83409.png)


| n_samples    | RNN            | Alergia       |train_files                                                              |
| :---         |     :---:      |       :---:   |                                                                  ---:   |
| 100          | 68.63%         | 68.63%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut113_100.dat  |
| 2000         | 100.00%        | 76.47%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut113_2000.dat |


for automaton
[blackbox.pdf](https://github.com/roiDaniela/run_time_verification/files/6971077/blackbox.pdf)
![image](https://user-images.githubusercontent.com/86918539/129101661-ded147eb-9ce5-4de9-acda-4b0c8e153222.png)

# (a+b)*abb

| n_samples    | RNN            | Alergia       |train_files                                                              |
| :---         |     :---:      |       :---:   |                                                                  ---:   |
| 100          | 64.52%         | 48.39%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut114_100.dat  |
| 2000         | 100.00%        | 80.65%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut114_2000.dat |

for automaton
[blackbox.pdf](https://github.com/roiDaniela/run_time_verification/files/6971302/blackbox.pdf)
![image](https://user-images.githubusercontent.com/86918539/129101722-2ec7f39e-998a-4b21-b129-c68b940d8604.png)

# ϵ|a*|b*a|(a|b)*abb(a|b)*abb

| n_samples    | RNN            | Alergia       |train_files                                                              |
| :---         |     :---:      |       :---:   |                                                                  ---:   |
| 100          | 91.00%         | 90.00%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut115_100.dat  |
| 2000         | 100.00%        | 93.00%        |https://github.com/pberko/al_rnn_results/blob/main/tracesaut115_2000.dat |


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
