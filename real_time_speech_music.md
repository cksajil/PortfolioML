# Real-Time Speech/Music Classification

### Project Details

A real-time Speech/Music Classification project using Deep Neural Network and Convolutional Network. The code for the project is available [here](https://github.com/cksajil/MusicRJ)

![Demo](https://github.com/cksajil/MusicRJ/blob/master/musicRJ.gif)

![Block diagram](https://i.ibb.co/5Y11jkp/Block-DGMSmall.png)

### Model 1 (Simple DNN) Architecture

```console
Model: "sequential"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 dense (Dense)               (None, 32)                8224                                                              
 dense_1 (Dense)             (None, 64)                2112                                                             
 dense_2 (Dense)             (None, 128)               8320                                                                  
 dense_3 (Dense)             (None, 256)               33024                                                                 
 dense_4 (Dense)             (None, 512)               131584                                                                 
 dense_5 (Dense)             (None, 256)               131328                                                                
 dense_6 (Dense)             (None, 128)               32896                                                                 
 dropout (Dropout)           (None, 128)               0                                                                    
 dense_7 (Dense)             (None, 64)                8256                                                             
 dense_8 (Dense)             (None, 2)                 130                                                                    
=================================================================
Total params: 355,874
Trainable params: 355,874
Non-trainable params: 0
_________________________________________________________________
```

![dnn architecture](https://github.com/cksajil/MusicRJ/blob/master/Images/dnn_model.png)


### Model 2 (CNN) Architecture

```console
Model: "sequential"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 conv2d (Conv2D)                (None, 101, 1290, 32)    320                                                                    
 max_pooling2d (MaxPooling2D)   (None, 50, 645, 32)      0                                             
 conv2d_1 (Conv2D)              (None, 48, 643, 64)      18496                                                              
 max_pooling2d_1 (MaxPooling2D) (None, 24, 321, 64)      0                                                                                       
 conv2d_2 (Conv2D)              (None, 22, 319, 64)      36928                                                                
 flatten (Flatten)              (None, 449152)           0                                                                   
 dense (Dense)                  (None, 64)               28745792                                                        
 dense_1 (Dense)                (None, 2)                130                                                            
=================================================================
Total params: 28,801,666
Trainable params: 28,801,666
Non-trainable params: 0
_________________________________________________________________
```
### [Click here to see complete demo video](https://www.youtube.com/watch?v=9X55T_ffNwg&t=685s)
