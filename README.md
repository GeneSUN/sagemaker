# sagemaker
This repository contains sagemaker related notebook, such as spark ETL, sklearn ETL, sagamaker training container 

A. xgboost_managed_spot_training.ipynb:
This notebook focus on Spot instance:
1. enable spot instance with train_use_spot_instances
2. Set up checkpoint: checkpoint_s3_uri
3. Train model with estimator, xgboost built-in container, AMT

B. scikit_learn_data_processing_and_model_evaluation.ipynb
This File contains "processing with sklearn" and "training/inference with own script and container"

C. feature_transformation_with_sagemaker_processing.ipynb
This file use 
1. build spark container for running processing job; 
2. write spark script process.py. 
3. lauch processing job with python SDK; 
4. lauch xgboost training job with python SDK.

D. autopilot_customer_churn.ipynb
1. Setting up Autopilot Job using boto3, with input_data_config, output_data_config, Problem_type, Training method, RoleArn
2. Analyzing Data, Feature Engineering, Model tuning
3. Generate notebook
4. look up best candidate with describe_auto_ml_job API
5. Deploy best_candidate with end_point
6. evaluate performance

E. keras_experiment.ipynb
AWS Experiment to monitor/track metrics
