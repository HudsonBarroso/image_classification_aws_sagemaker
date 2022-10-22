# Image Classification using AWS SageMaker

Use AWS Sagemaker to train a pretrained model that can perform image classification by using the Sagemaker profiling, debugger, hyperparameter tuning and other good ML engineering practices. This can be done on either the provided dog breed classication data set or one of your choice.

## Dataset
The provided dataset is the dogbreed classification dataset

### Access
Upload the data to an S3 bucket through the AWS Gateway so that SageMaker has access to the data. 

## Hyperparameter Tuning
I choosed the pretrained model ResNet-18, it has been trained on a subset of the ImageNet database. The model is trained on more than a million images, and can classify images into 1000 object categories

We tuned three hyperparameters.

1. lr: Learning Rate, It scales the magnitude of the model's weight updates in order to minimize the model's loss
2. weight-decay: Controls the degree of the regularization (the larger the stronger) and is applied universally to all learned parameters of the model by default
3. batch-size: Is defined as the number of samples processed before the model is updated.

Hyperparameter Tuning Job
![Hyperparameter Tuning Job](hp_tunning.png?raw=true "Hyperparameter Tuning Job")

Hyperparameter Tuning Metrics
![Hyperparameter Tuning Metrics](hp_tunning_log_metrics.png?raw=true "Hyperparameter Tuning Metrics")

Training Job Output
![Training Job Output](training_result_v2.png?raw=true "Training Job Output")


## Debugging and Profiling
**TODO**: Give an overview of how you performed model debugging and profiling in Sagemaker

### Results
**TODO**: What are the results/insights did you get by profiling/debugging your model?

**TODO** Remember to provide the profiler html/pdf file in your submission.


## Model Deployment
**TODO**: Give an overview of the deployed model and instructions on how to query the endpoint with a sample input.

**TODO** Remember to provide a screenshot of the deployed active endpoint in Sagemaker.

## Standout Suggestions
**TODO (Optional):** This is where you can provide information about any standout suggestions that you have attempted.
