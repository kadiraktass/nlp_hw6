## Neutral language processing HW6

Link to my github repo for this hw: https://github.com/kadiraktass/nlp_hw6

# STEP 1

I could only manage to use baseline model and ELMO model. 

For baseline model:  
  Training accuracy = 0.950  
  Validation accuracy = 0.357  

For ELMO model:  
  Training accuracy = 0.530  
  Validation accuracy = 0.432  
  
I choose ELMO model to continue. Because it has less overfitting and better validation accuracy.  

Config for the baseline model: https://github.com/kadiraktass/nlp_hw6/blob/master/baseline_config.json  
Config for the ELMO model: https://github.com/kadiraktass/nlp_hw6/blob/master/elmo_config.json  

# STEP 2
I had overfitting.  As you can see in the graph, the gap between training accuracy is much more higher than validation accuracy.  
![alt text](https://github.com/kadiraktass/nlp_hw6/blob/master/legend.png)  
![alt text](https://github.com/kadiraktass/nlp_hw6/blob/master/acc_before.png)  
![alt text](https://github.com/kadiraktass/nlp_hw6/blob/master/loss_before.png)  

Changes:  
1) Epoch number is decreased from 20 to 5. Patience is decreased from 5 to 1.  
  Training accuracy = 0.451  
  Validation accuracy = 0.429  
2) Batch size is increased from 32 to 128.  
  Training accuracy = 0.423  
  Validation accuracy = 0.422  
3) Hidden dim is increased from 128 to 256  
  Training accuracy = 0.390  
  Validation accuracy = 0.416  
4) Hidden dim is decreased from 256 to 64  
  Training accuracy = 0.407  
  Validation accuracy = 0.407  
 
 After these trials, I picked the best hyperparameters I observed.  
  Training accuracy = 0.423  
  Validation accuracy = 0.422  
 Compared to before overfitting is reduced. Actually, we can say that there is not an overfitting anymore.  
 On the other hand, validation accuracy decreased.  
 However, it is ok, because we got rid of overfitting by sacrificing just a little bit of validation accuracy.  
 Config file with new hyperparameters: https://github.com/kadiraktass/nlp_hw6/blob/master/elmo_changed_config.json   
 After changes:  
![alt text](https://github.com/kadiraktass/nlp_hw6/blob/master/legend.png)  
![alt text](https://github.com/kadiraktass/nlp_hw6/blob/master/acc_after.png)  
![alt text](https://github.com/kadiraktass/nlp_hw6/blob/master/loss_after.png)  

 
 # STEP 3
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
