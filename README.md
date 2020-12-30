# ML engineer for Azure nanodegree - project 2 by S.Korhonen

This project entailed deploying two machine learning models. First was created and deployed using Azure UI and the second through jupyter notebook in SDK. 
For the first, also documentation was implemented using Swagger and performance was benchmarked.

## Architectural Diagram
![architectural diagram of project2](/screenshots/Architectural_diagram)

## Key Steps
*TODO*: Write a short discription of the key steps. Remeber to include all the screenshots required to demonstrate key steps. 
As seen in the architectural diagram above, there were several key steps to this project. First I created a compute instance to explore the dataset.
![](/screenshots/Compute-instance-running)
Then I created a compute cluster for modelling and deployment for this project.
![](/screenshots/Cluster-running)
Thirdly I imported the Bankmarketing dataset to Azure to be able to model it and also profiled it to get a feel for the data.
![](/screenshots/Bankmarketing-data-in-azure)
Then I trained the AutoML model.
![](/screenshots/completed_automl_run1)
After the AutoML was finished, I selected the best model, which was the VotingEnsemble and deployed it with authentication.
![](/screenshots/Best_model_run1_deployed)
I enabled application insights, to be able to view the goings of this model in deployment.
![](/screenshots/Application_insights_enabled)
I created Swagger documentation to help interact with the model through the REST API endpoint.
![](/screenshots/Swagger_on_localhost)
![](/screenshots/Swagger_get)
![](/screenshots/Swagger_post)
![](/screenshots/Swagger_responses)
Finally I consumed the endpoint of the deployed model.
![](/screenshots/Running_endpoint_API_call)

After all this was done, I recreated the project with SDK.
![](/screenshots/SDK_running_pipeline)
![](/screenshots/SDK-pipeline_running)
![](/screenshots/SDK_pipeline_run_overview)
![](/screenshots/SDK_Models_running)
![](/screenshots/SDK_Bankmarketing_train_finished_run)
![](/screenshots/SDK_automl_endpoint)
![](/screenshots/SDK_automl_overview)
![](/screenshots/SDK_active_endpoint)
![](/screenshots/SDK_deployed_active_endpoint)
![](/screenshots/SDK_rundetails_widget)

## Screen Recording
My screen recording of the project can be found here: [](https://youtu.be/IFRC-Co59mY)

## Standout Suggestions
I benchmarked my deployed model as seen in image below.
![](/screenshots/benchmark)
