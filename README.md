# cse598-002

For each of the code files, you will need to install the simglucose repository for the functional imports to work. 
Otherwise, the conditional diffusion code should be self contained and work with common python packages. 

The wandb login codes will need to be changed to reflect future user's account, otherwise sections of the training code may not function correctly. 
At the start of the training function, you can define a few hyperparameters and key variable sizes. Refer to where those variables are called in the code to determine if or when it is appropriate to change their numbers. 
The action dimension should always be 1, as our model is not meant to calculate basal insulin actions. 
