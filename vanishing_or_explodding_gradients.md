- training model overtime leads to exponentailly small/larrge gradients
- note this is the output of a NN:
![output](https://i.gyazo.com/7c2dacf929b385ebf17fb40592c2c6c5.png)
  - therefore if the weights are just larger than the Identity matrix, then [some math arg can be made that] deriv will icnrease exponentially
  - same v.v.

## partial solution
  - weight random initialization
  - let n[l] be # of neurons in layer l
![weights](https://i.gyazo.com/090473ed8f7644ba2e22801627919bf2.png)

