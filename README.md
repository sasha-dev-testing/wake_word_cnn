# wake_word_cnn

A repo with a test task to build a Wake Word model, using "STOP" as a trigger. 

To test the model:

```wget https://testing-wakeword.s3.us-east-2.amazonaws.com/wake_word_stop_model.h5``` and specify the path in the notebook.

To train the model, avoiding MFCC extraction, first download MFCC features:

```wget https://testing-wakeword.s3.us-east-2.amazonaws.com/all_targets_mfcc_sets.npz```, specify the path then start from the "Settings" part of the notebook. 

The model for now has 98% accuracy and also can be converted to *.tflite format to be deployed on any small single-board computers, such as Raspberry Pi.

I hope that this solution will be interesting, and I'm ready to discuss each part of the code. 
