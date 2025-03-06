#GSynergy Data Engineer Interview Challenge

To run this code successfully without any failures, follow the steps below:

Create an Azure Account

Set up an Azure Storage Account:
Create a storage account named gsynergydatastore.
Inside it, create a container named raw-data.
Upload all the challenge assets to the raw-data container in .dlm.gz format.

Create an Azure Databricks Service:
Name it gsynergy-databricks.
Launch the service after creation.

Set up the Workspace in Databricks:
Inside the Workspace directory, create a folder named gsynergy.
Create the following notebooks inside this folder and paste the corresponding code:
SecretsNotebook
1.Mount_Storage
2.Transformation
3.Incremental_Load

Retrieve the Storage Account Access Key:
Go to Security + Networking → Access Keys in the Azure portal.
Copy the access key for gsynergydatastore.

Update the Secrets Notebook:
Replace storage_account_key with the access key obtained in the previous step.

Run the Transformation Notebook:
This will automount the storage and transform the data as required for the challenge.
