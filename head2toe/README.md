# cmpe297_hw3

The new transfer learning model, Head2Toe, takes the advantages of linear probing and fine-tuning. The key is to select important features from all layers in the model to train a classification head for the target-domain. It takes all the pre-trained layers' outputs, and then apply a linear layer to predict final output. The goal is to imporve linear probing, and reduce computation of fune-tuning, which overall for imporving transfer learning.
</br>
</br>
I tried two model configuration: one with fune-tuning only, one with Head2toe. </br>
The dataset I used is imagenetr50, it contains 50 training images per class. This dataset often used for image classification. </br>
The result from fune-tuning: </br>
{'support_loss': 0.00026232834, 'support_accuracy': 0.03125, 'query_loss': 0.0006715605, 'query_accuracy': 0.08} </br>
The result from Head2toe: </br>
{'support_loss': 1.7136148e-07, 'support_accuracy': 0.03125, 'query_loss': 4.3868536e-07, 'query_accuracy': 0.08} </br>
In summary, the result from head2toe has less loss; it increases efficiency of fine-tunning and accuracy of linear probing.

For further exploration, you can test it with other pre-trained model, imagenetvitB16. </br>

Colab Link: https://colab.research.google.com/drive/1Ij8sFL4a5GjDHntJgWiGrel0t6jfUaqP
