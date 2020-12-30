# ML engineer for Azure nanodegree - project 2 by S.Korhonen

This project entailed deploying two machine learning models. First was created and deployed using Azure UI and the second through jupyter notebook in SDK. 
For the first, also documentation was implemented using Swagger and performance was benchmarked.

## Architectural Diagram
![architectural diagram of project2](/screenshots/Architectural_diagram.png)

## Key Steps
*TODO*: Write a short discription of the key steps. Remeber to include all the screenshots required to demonstrate key steps. 
As seen in the architectural diagram above, there were several key steps to this project. First I created a compute instance to explore the dataset.
![](/screenshots/Compute-instance-running.png)
Then I created a compute cluster for modelling and deployment for this project.
![](/screenshots/Cluster-running.png)
Thirdly I imported the Bankmarketing dataset to Azure to be able to model it and also profiled it to get a feel for the data.
![](/screenshots/Bankmarketing-data-in-azure.png)
Then I trained the AutoML model.
![](/screenshots/completed_automl_run1.png)
After the AutoML was finished, I selected the best model, which was the VotingEnsemble and deployed it with authentication.
![](/screenshots/Best_model_run1_deployed.png)
I enabled application insights, to be able to view the goings of this model in deployment.
![](/screenshots/Application_insights_enabled.png)
I created Swagger documentation to help interact with the model through the REST API endpoint.
![](/screenshots/Swagger_on_localhost.png)
![](/screenshots/Swagger_get.png)
![](/screenshots/Swagger_post.png)
![](/screenshots/Swagger_responses.png)
Finally I consumed the endpoint of the deployed model.
![](/screenshots/Running_endpoint_API_call.png)

After all this was done, I recreated the project with SDK.
![](/screenshots/SDK_running_pipeline.png)
![](/screenshots/SDK-pipeline_running.png)
![](/screenshots/SDK_pipeline_run_overview.png)
![](/screenshots/SDK_Models_running.png)
![](/screenshots/SDK_Bankmarketing_train_finished_run.png)
![](/screenshots/SDK_automl_endpoint.png)
![](/screenshots/SDK_automl_overview.png)
![](/screenshots/SDK_active_endpoint.png)
![](/screenshots/SDK_deployed_active_endpoint.png)
![](/screenshots/SDK_rundetails_widget.png)

## Screen Recording
My screen recording of the project can be found here: [](https://youtu.be/IFRC-Co59mY)

## Future Improvements for the project
The time limitation in this project left me very little time to go over the actual data and, while the same data was used in the previous project, this is one area
of improvement I want to point out. Machine learning models are best done understanding the data, the predictions and the process. I
would also improve on trying out different parameters in the pipelines and also different options in the deployment and publication.

## Standout Suggestions
I benchmarked my deployed model as seen in image below.
![](/screenshots/benchmark.png)
