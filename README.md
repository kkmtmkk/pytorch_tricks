# pytorch_tricks
1. Check the type of data carefully. Small differences will make slight decrease in accuracy.
2. Out of distribution input may affect the performance of network because of batch normalization.
3. Pay attention to different kinds of experients. It's better to put them in different files because annotation may mess up.
4. Use state_dict routines to load models for different version training. Simple torch.load is not okay.
5. When writing programs about gradients, try to think about corresponding computing graphs to ensure everything is under control.
6. Make sure all the parameters are put into the optimizer. Pay attention to the case when modifying several layers between training.
7. Remember to use handle.remove() after implementing layer.register_forward_hook() to get intermediate features. copy.deepcopy() will retain register_forward_hook.
8. vector.register_hook() will be called once the vector appears. Pay attention to the special cases when it appears in different networks.
