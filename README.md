# flask-ml-AzureDevOps-serverless
Performing machine learing task with flask and Azure Devops; everything is running to serverless

## Set Up Azure Pipelines

- Launch Cloud shell
- Set up the GitHub Repo and integrate Azure Pipelines from the GutHub Marketplace
- Clone this repository in the enviroment
- ```cd``` into the directory
```
cd flask-ml-AzureDevOps-serverlss
```
- Set up a virtual enviroment 
```
python3 -m venv ~/.flask-ml-AzureDevOps
source ~/.flask-ml-AzureDevOps/bin/activate
```
- Run the ```make install``` command to install the dependencies from the ```makefile```.
- Create an app service and deploy as well then verify 
```az webapp up -n <your-appservice>```; choose any name for your appservice. Verify by running the link in your browser 
```
https://<your-appservice>.azurewebsites.net/
```
- Perform prediction by changing the  ```make_predict_azure_app.sh``` file to match the app service URL
- Create an Azure DevOps Project using this [documentation](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?view=azure-devops)
- Set up a Continuous Delivery Workflow following this [documentation](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?view=azure-devops) as well. The good thing is the template has it all figured out for your application. 
- Check your build and confirm it's working, probably get a status badge and update your READme

## Note
All the steps mentioned are just to perform a simple deployment with the Azure Pipeline and a demo project. The steps does not vary with other types of applications; the goal of the repo is to explore Azure Pipelines not neccesarily the application type. 

## Hire me
Looking for an engineer to build and automate your next application infrastruture/architecture to work remotely? Get in touch: sbayo971@gmail.com

## How can I thank you?
Why not star the Github repo? I'd love the attention! Why not share the link for this repository on Twitter,Hackernews or Destructoid ? Spread the word!

Don't forget to follow me on [twitter](https://twitter.com/SamuelArogbonlo). Also, you could see other things I do in the software enviroment via my [website](https://samuelarogbonlo.github.io/)
