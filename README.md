# Purpose & description
Tasks to help with the rights assignation between Azure Kubernetes Cluster instance and Azure Container Registry. See ***[Release notes](https://github.com/expertasolutions/AzureContainerRegistryExtensions/releases)***

# Prerequisites to be used
The **Service Principal** used with your Azure Service Connection endpoint need to be 'Owner' of you **Azure subscription** where your **Azure Container Registry** is created.


# Tasks include

**NOTE**: ***AdminUser*** must be enable on your Azure Container Registry to used this task.

## ACRCredentials
![ACRCredentials](_screenShots/ACRCredsInfo-v0.png)

#### Action Type
- Show: Get the current credentials information
- Renew: Renew the current credentials information access
#### Output variables
- username
- password
- password2

## ACRAKSAccess

![ACRAKSAccess](_screenShots/ACRAKSAccess-v0.png)

#### Access Mode
- RBAC
- AKS Secret
- AKS Service Account ([already plan](https://github.com/expertasolutions/AzureContainerRegistryExtensions/issues/9))

#### Output variables
- imagePullSecretName