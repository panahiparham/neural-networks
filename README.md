# neural-networks
implementing neural networks from scratch


# Part 1 - oldschool backprop

*code* ->  `oldschool_backprop.ipynb`<br/>
*math* ->(oldschool_backprop_math.pdf)[https://drive.google.com/file/d/1CyWY_l45qt3L472i1gKYZZ-1p_kI1CZ-/view?usp=sharing]
*paper notes* -> `1986_paper_notes.pdf`<br/>
 * Create, train and evaluate feed forward neural networks, as it was described in the 1986 paper - [learning representations by back-propagating errors](https://www.iro.umontreal.ca/~vincentp/ift3395/lectures/backprop_old.pdf).


* This code follows how backprop was described in the paper, meaning that derivatives are calculated per training example per node per layer, without any vectorization. That fact makes training very slow in comparison to modern implementations of neural networks.

* This project is a personal investigation into how it would have probably felt like to train a neural network before the age of GPU powered deep learning or efficient computing tricks.

* Next step is coding up a modern implementation of backprop taking advantage of matrix calculus and vectorization.


### overall structure

  - initialize model parameters

  - repeat until convergence
    - forward propagation 
    - cost computation
    - backward propagation
    - updating parameters
  - evaluate network

  - perform predictions

Btw. you can find links to my paper summary and rederivation of backprop in pdf format at the top of this page. If you saw any mistakes in math or code please let me know, I'm learning and I highly appreciate any tips or advise :)

### results

- here are some results from training neural nets on some synthetic datasets. checkout `oldschool_backprop.ipynb` for implementation.
<br/>

---
- dataset 1

![](https://github.com/panahiparham/neural-networks/blob/main/assets/p1_r1_1.png?raw=true)

```
 == Training == 
cost after epoch 100 -  12.375031118691
cost after epoch 200 -  10.563136027274641


 == Evaluation == 
cost: 10.556284775290768  - accuracy: 0.94

Training took 78.75 seconds.
```
![](https://github.com/panahiparham/neural-networks/blob/main/assets/p1_r1_2.png?raw=true)
![](https://github.com/panahiparham/neural-networks/blob/main/assets/p1_r1_3.png?raw=true)

---
- dataset 2

![](https://github.com/panahiparham/neural-networks/blob/main/assets/p1_r2_1.png?raw=true)

```
 == Training == 
cost after epoch 100 -  12.375031118691
cost after epoch 200 -  10.563136027274641


 == Evaluation == 
cost: 10.556284775290768  - accuracy: 0.94

Training took 78.75 seconds.
```
![](https://github.com/panahiparham/neural-networks/blob/main/assets/p1_r2_2.png?raw=true)
![](https://github.com/panahiparham/neural-networks/blob/main/assets/p1_r2_3.png?raw=true)

---
- dataset 3

![](https://github.com/panahiparham/neural-networks/blob/main/assets/p1_r3_1.png?raw=true)

```
 == Training == 
cost after epoch 100 -  12.375031118691
cost after epoch 200 -  10.563136027274641


 == Evaluation == 
cost: 10.556284775290768  - accuracy: 0.94

Training took 78.75 seconds.
```
![](https://github.com/panahiparham/neural-networks/blob/main/assets/p1_r3_2.png?raw=true)
![](https://github.com/panahiparham/neural-networks/blob/main/assets/p1_r3_3.png?raw=true)
<br/>
