# Steps to setup Azure App Service

1. Login Azure Hothouse
- az login -t 6bb1947d-170d-407c-a557-34a5e3f286ce

2. Create Azure Resource Group
- az group create --name group-name --location some-location

3. Deploy Custom Template to Azure Resouce Group
- az deployment group create --resource-group group-name --template-uri path-to-json-raw-file

4. Add azure-webapp-maven plugin and configure settings
- refer to https://docs.microsoft.com/en-us/azure/developer/java/spring-framework/deploy-spring-boot-java-app-with-maven-plugin

5. Build and Deploy
- mvn clean package
- mvn azure-webapp:deploy
