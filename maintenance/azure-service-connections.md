# Updating Azure Service Connection in Azure Devops.

When Azure Service Connection keys are expired, pipelines will fail and give the following error.   
  
`Azure login failed`  
`The provided client secret keys for app *** are expired.`

![](https://user-images.githubusercontent.com/114651675/219621483-de7c361a-7c7f-4e40-8c87-048ee73d42d8.png)

  
  
Here's how to update the Azure connection.  
  
Go to Azure Devops dashboard.   
Select the project and go to project settings. (Bottom left corner)  
Go to **Service Connections** menu.  
Select **Planpod (**_subscription id_**)** and click on **Manage Service Principal** link.  
This will take you to azure active directory portal and open up the service account settings.  
Now go to **Certificates & Secrets** blade.  
Click on **New client secret** to create a new secret.  
Go back to Azure Devops settings page. (And to Service connections and select the connection)  
Click on Edit button in top right.  
Click **Save** edit drawer.  
Once drawer is closed refresh the page.  
Click edit again.  
This time click on **Verify** and make sure everything is okay.
