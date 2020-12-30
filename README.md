# ML engineer for Azure nanodegree - project 2 by S.Korhonen

This project entailed deploying two machine learning models. First was created and deployed using Azure UI and the second through jupyter notebook in SDK. 
For the first, also documentation was implemented using Swagger and performance was benchmarked.
I downloaded the data from a provided link, imported it to Azure as a dataset. Then I utilised the AutoML in Azure to create the best possible
classification model it could find. The best model created was deployed as a webservice that can be utilised from anywhere that can communicate via HTTP.

## Architectural Diagram
![architectural diagram of project2](/screenshots/Architectural_diagram.png)

## Key Steps
As seen in the architectural diagram above, there were several key steps to this project. First I created a compute instance to explore the dataset.
![](/screenshots/Compute-instance-running.png)

Then I created a compute cluster for modelling and deployment for this project.
![](/screenshots/Cluster-running.png)

Thirdly I imported the Bankmarketing dataset to Azure to be able to model it and also profiled it to get a feel for the data.
![](/screenshots/Bankmarketing-data-in-azure.png)
![](/screenshots/Registered_dataset.png)

Then I trained the AutoML model.
![](/screenshots/completed_automl_run1.png)
![](/screenshots/experiments_completed.png)

After the AutoML was finished, I selected the best model, which was the VotingEnsemble and deployed it with authentication.
![](/screenshots/Best_model_run1_deployed.png)

I enabled application insights, to be able to view the goings of this model in deployment.
![](/screenshots/Application_insights_enabled.png)

I ran logs.py to make sure my model created logs.
![](/screenshots/Logs_running.png)

I created Swagger documentation to help interact with the model through the REST API endpoint.
![](/screenshots/Swagger_on_localhost.png)
![](/screenshots/Swagger_get.png)
![](/screenshots/Swagger_post.png)
![](/screenshots/Swagger_responses.png)

Finally I consumed the endpoint of the deployed model.
![](/screenshots/Running_endpoint_API_call.png)

After all this was done, I recreated the project with SDK. I ran the pipeline from jupyter notebook.
![](/screenshots/SDK-pipeline_running.png)

I used the same data and used the automl module.
![](/screenshots/SDK_pipeline_run_overview.png)

It ran several different models while attempting to maximize accuracy.
![](/screenshots/SDK_Models_running.png)

It finished modelling, selected the best model and deployed the model for consumption.
![](/screenshots/SDK_Bankmarketing_train_finished_run.png)
![](/screenshots/SDK_automl_endpoint.png)
![](/screenshots/SDK_automl_overview.png)

Here is the pipeline as seen from Azure.
![](/screenshots/SDK_running_pipeline.png)
![](/screenshots/pipeline_runs_asseenfromAzure.png)

These two screenshots show the active endpoint from notebooks and Azure.
![](/screenshots/SDK_active_endpoint.png)
![](/screenshots/SDK_deployed_active_endpoint.png)

I had enabled the runDetails widget.
![](/screenshots/SDK_rundetails_widget.png)

All in all I did three experiments including exploring the dataset.
![](/screencasts/all_experiments.png)

And created two pipelines as seen in image below.
![](/screencasts/Both_pipelines.png)

## Screen Recording
My screen recording of the project can be found [here on Youtube](https://youtu.be/IFRC-Co59mY)

The video does not, unfortunately, show the pipeline endpoint section, so the screenshot above shows that.

Also please check my first take video containing the endpoint more clearly. It missed the audio, so I had to rush the second video a bit. The first video
can be found [here on Youtube](https://youtu.be/WeSCx7MXDtc)

## Future Improvements for the project
The time limitation in this project left me very little time to go over the actual data and, while the same data was used in the previous project, this is one area
of improvement I want to point out. Machine learning models are best done understanding the data, the predictions and the process. I
would also improve on trying out different parameters in the pipelines and also different options in the deployment and publication.

## Standout Suggestions
I benchmarked my deployed model as seen in image below.
![](/screenshots/benchmark.png)
