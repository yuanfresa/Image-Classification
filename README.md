# Image-Classification
Udacity Deep Learning Nanodegree Project 2
## Weight Initialization Matters
``` 
weight = tf.Variable(tf.truncated_normal([*conv_ksize, x_tensor.get_shape().as_list()[-1], 
                                              conv_num_outputs],stddev=0.05))
```
When I use the default standard deviation(stddev=1) to initialize the filters' weights, the validation accuracy stays at 10% and did not change at all.
