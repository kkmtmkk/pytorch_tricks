# pytorch_tricks
1. Check the type of data carefully. Small differences will make slight decrease in accuracy.
2. Out of distribution input may affect the performance of network because of batch normalization.
3. Pay attention to different kinds of experients. It's better to put them in different files because annotation may mess up.
4. Use state_dict routines to load models for different version training. Simple torch.load is not okay.
