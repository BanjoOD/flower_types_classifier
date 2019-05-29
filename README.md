# flower_types_classifier
Convolutional neural network to identify flower types from images
*This was also project during my Udacity course 
*I used Pre-trained CNN models to train a network that identifies 102 classes of flowers with up to 92.3% testing accuracy.
*The classifier trains the network, creates a checkpoint which is used to reload the saved network during prediction
*I used pytorch libraries for training and prediction
*The codes files are available in jupyter notebook and as a script

To run the train script:
                  python train.py data_directory [options]
 
    --save_dir       :directory to save checkpoint
    --arch           :Pretrained Network model to be used choices = [densenet, resnet, vgg]
    --lr             :learning rate
    --epochs         :Epoch
    --device         :device to train with: cuda or cpu
    --hidden_units   :hidden units to  be used in the classifier training
    --top_k          :top K classification probability
    --cat_to-names   :category to names mapping
    
    
To run the predict script:
                    python predict.py path/to/image checkpoint_dir [options]
                    
    --top_k           :top K classification probability
    --cat_to-names    :category to names mapping
    --device          :device to use: gpu or cpu
