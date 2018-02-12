## Ising model phase transition with CNN

This is a short notebook to reproduce some results from [this paper](https://arxiv.org/pdf/1605.01735.pdf).

More details are in the python notebook, but in brief, 2D Ising model spin configurations are generated
by Monte Carlo and then used to train a convolutional neural network. The CNN is trained only on configurations 
deep within the ordered or disordered phases (very high or very low temperatures). It is then tested on
configurations across a range of temperatures including near the critical regime. In essence, the CNN
can classify a given spin configuration as belonging to the ordered or disordered phase and predicts an
accurate critical temperature.


### Instructions
* Fairly common dependencies: numpy, matplotlib, scikit, scipy, keras, tqdm
* For keras, there are a few lines that assume tensorflow as the backend, but they are easily modified
* Clone and run with something like `jupyter notebook`

