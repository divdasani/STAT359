# STAT359
Repo for STAT359 Capstone

## Summary
I worked on model training and deployment (CI/CD) throughout the quarter. My work focised on building, training, and deploying the model for continuous serving. This is vital to the infrastructure as the inferencing model will be used by the application to make time series predictions. As we gather data and can develop more powerful models, we need a way to deploy them in a manner that allows for contiuous service to our clients in real-time, which the Sagemaker based CI/CD pipeline allows. This part of the project is vital because it connects the backend together and uses the information and data compiled by the other microservices to serve the users requests.

## Reproduction
1. Create AWS Account
2. Create an S3 bucket (ensure your region is US-West)
3. Create a Sagemaker instance
a. Set IAM permissions for notebook to full Sagemaker Access
b. Select clone git repo, and copy the URL of this repo and paste it there
4. Open Jupyter Notebook in Sagemaker and change bucket name to the one you created in (2)
5. Run!

## Big Picture
PredicT relies on employing data to predict future time series events. All this is done by the model in Sagemaker. This model not only allows for low-latency, high reliability inferencing, but is also deployed in a nature that allows for easy scalability and easy CI/CD. One  way this module can be further improved is by adding an ensemble of models that work in conjunction for prediction. Another way is to create model package architecture that allows for seamless model swapping and interchanging.

