# Bayesian-network-weighted-and-Gibbs-sampling-
Bayesian network implementation using weighted and Gibbs sampling

The network example used looks like that:

![Network](/image/network.png)

The input format for that network is:

` rede = BayesNet([('B', '', 0.9),
                   ('M', '', 0.1),
                   ('I', 'B M', {(T, T): 0.9, (T, F): 0.5, (F, T): 0.5, (F, F): 0.1}),
                   ('G', 'B I M', {(T, T, T): 0.9, (T, T, F): 0.8, (T, F, T): 0.0, (T, F, F): 0.0, (F, T, T): 0.2, (F, T, F): 0.1, (F, F, T): 0.0, (F, F, F): 0.0}),
                   ('J', 'G', {T: 0.9, F: 0.0}),]) `
                 
You can adapt to any desired input.           
