# Steps to setup Azure App Service

1. Login Azure Hothouse
- az login -t 6bb1947d-170d-407c-a557-34a5e3f286ce

2. Create Azure Resource Group
- az group create --name group-name --location some-location

3. Deploy Custom Template to Azure Resouce Group
- az deployment group create --resource-group group-name --template-url path-to-json-url