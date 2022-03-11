# ML.NET

---------------------------------------------------------
## ML.NET Model Builder is an intuitive graphical Visual Studio extension to build, train, and deploy custom machine learning models.
Model Builder uses automated machine learning (AutoML) to explore different machine learning algorithms and settings to help you find the one that best suits your scenario.<br />

## Select Image Classification Scenario
![](Images/01-Scenarios.PNG)<br />
## Select Trainning Environment
![](Images/02-Scenarios.PNG)<br />
## Once you have chosen your scenario, Model Builder asks you to provide a dataset
![](Images/03-Data.PNG)<br />
## Train
![](Images/04-Training.PNG)<br />
## In my case, this training lasted a little over 4 hours
![](Images/05-Training-Results.PNG)<br />
## Evaluate
![](Images/06-Evaluate.PNG)<br />
![](Images/07-Evaluate-Test.PNG)<br />
![](Images/08-Evaluate-Result.PNG)<br />
## Consume
![](Images/09-Consume.PNG)<br />
## Add solution ConsoleApp and WebApi<br />
![](Images/10-AddSolutions.PNG)<br />


## OPEN PowerShell and Test your WebAPI<br />
> $body = @{ImageSource = "Image location on your local machine"<br />
> Invoke-RestMethod "https://localhost:'PORT'/predict" -Method Post -Body ($body | ConvertTo-Json) -ContentType "application/json"<br />

### DataSet: https://www.kaggle.com/muhammadshahzadkhan/dogvscat

# ML.NET Documentation
>https://docs.microsoft.com/en-us/dotnet/machine-learning/<br />
>https://dotnet.microsoft.com/apps/machinelearning-ai/ml-dotnet/model-builder
