---
title: "Quickstart: Create a Python project from a template in Visual Studio | Microsoft Docs"
ms.custom: ""
ms.date: 09/25/2017
ms.reviewer: ""
ms.suite: ""
ms.technology:
  - "devlang-python"
ms.devlang: python
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 3f4b66c5-3ad8-4067-90cd-0100205700a7
caps.latest.revision: 1
author: "kraigb"
ms.author: "kraigb"
manager: ghogen
---

# Quickstart: create an AI project from the Azure Machine Learning Gallery in Visual Studio

Azure Machine Learning is integrated with Visual Studio Tools for AI. You can use it to submit machine learning jobs to remote compute targets like Azure virtual machines, Spark clusters, and more. Learn more about [Azure Machine Learning Experimentation](https://docs.microsoft.com/en-us/azure/machine-learning/preview/experimentation-service-configuration) 

Once you've [installed Visual Studio Tools for AI](installation.md), it's easy to create a new Python project using pre-made recipes in the Azure Machine Learning Sample Gallery.

> ! Azure Machine Learning Workbench must be installed. To install it please see the [Azure Machine Learning installation quickstart](https://docs.microsoft.com/en-us/azure/machine-learning/preview/quickstart-installation) 

1. Launch Visual Studio. Open the **Server Explorer** by opening the **AI Tools** menu and choosing **Select Cluster**	

    ![Cluster chooser](media/select-cluster.png)

1. Sign in to your Azure Machine Learning subscription by right-clicking the **Azure Machine Learning** node in the Server Explorer then select **Login** and follow the directions.

    ![login](media/azureml-login.png)
 
2. Select **AI Tools > Azure Machine Learning Sample Gallery**. 
	
    ![Sample gallery](media/gallery.png)

1. For this Quickstart, select the "**MNIST using TensorFlow**" sample and click **Install**. Provide the 
2.
 - **Resource Group**: Azure resource group where your metadata will be stored
 - **Account**: Azure Machine Learning experimentation Account
 - **Workspace**: Azure Machine Learning workspace
 - **Project Type**: The machine learning framework. In this case choose **TensorFlow**
 - **Add to Solution**: determines whether to add to your current Visual Studio Solution or a create and open a new solution
 - **Project Path**: Location to save the code
 - **Project Name**: Type **TensorFlowMNIST**
   

    ![Resulting project when using the Python Application template](media/new-AzureSampleProject.png)

1. Visual Studio creates the project file (a `.pyproj` file on disk) along with other files defined in the sample. With the "MNIST" template, the project contains several files.

    ![mnist](media/azml-mnist.png)

1. Submit the job to Azure Machine Learning. 

    ![mnist](media/submit-azml.png)

1. Run in a Docker container or on your local machine

    ![mnist](media/azml-local.png)