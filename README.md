# robond project 4: follow me



##### completion requirements



1. Fill out the following code blocks:

   Encoder block:

   ``` python
   def encoder block(input_layer, filters, strides):
       
   	# create a separate convolution layer using the
       # separable_conv2d_batchnorm() function
       
       return output_layer
   ```

   Decoder block:

   ```python
   def decoder block(small_ip_layer, large_ip_layer, filters):
     
     # upsample the small input layer using the bilinear_upsample() function
     
     # concatenate the upsampled and large input layers using layers.concatenate
     
     # add some number of separate convolution layers
     
     return output_layer
   ```

   Network:

   ```python
   def fcn_model(inputs, num_classes):
       
       # add encoder blocks
       # with each encoder layer, the depth of your model (number of filter)
       # increases
       
       # add 1x1 convolution layer using conv2d_batchnorm()
       
       # add same number of decoder blocks as the number of encoder blocks
       
       # the function returns the output layer fo the model
       # "x" is final layer obtained from the last decoder_block()
       
       return layers.Conv2D(num_classes, 1, activation='softmax', padding='same')(x)
   ```

   ​

2. Optimize the network and hyper-parameters

   ```python
   learning rate = 0
   batch_size = 0
   num_epochs = 0
   steps_per_epoch = 200
   validation_steaps = 50
   workers = 2
   ```

   ​

3. Train network and achieve accuracy of 40% using the Intersection over Union IoU metric (`final_grade_score`) 

   ​

4. Create brief writeup