# cmpe297_hw3

MMoE is the multi-task laerning model implemented by Google in 2018.</br> 
![image](https://user-images.githubusercontent.com/32551600/197459037-8cd4cb10-b683-4a0f-a1f4-fc0e3a5f5009.png) </br>
Multi-gate MoE model (MMoE)：uses bottom layers' sharing so that inductive bias can work better. In MMoE, every task/target has its own gate. Every task sharing all the experts (expert = fully connected layers). A gate is used to adjust signal ratio from the experts. </br>
The MMoE model I used has 14544 parameters. And after 100 epoches, the result are: </br>
validation loss is 0.0435 </br>
vallidation y0 loss is 0.0218 </br>
validation y1 loss is 0.0217 </br> 
validation y0 MAE is 0.1175 </br> 
validation y1 MAE is  0.1181 </br>

Colab Link: https://colab.research.google.com/drive/1jfbUDrrQ5Xpu-xDu0KqKg4R9OeZRAsNf#scrollTo=dUDwrINlwlCa
