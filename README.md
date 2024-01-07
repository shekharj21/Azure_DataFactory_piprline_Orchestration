# Azure_DataFactory_pipeline_Orchestration

## Project architecture :

![Screenshot (486)](https://github.com/shekharj21/shekharj21/assets/54074505/a00853b0-135f-4cac-96d5-9f1dc02b64e1)
1. ADLS : We will be using ADLS as an input the Data into the Azure Data Factory.
2. Azure Data Factory : We will be using azure datafactory to transform the data and for orchestration purpose.
3. AZURE SQL : As a Destination to dump the data.

## Create a Resource group :
1. Create a resource group in azure portal.
2. Its all the simple information.

## Deploy Storage Account :


![Screenshot (487)](https://github.com/shekharj21/shekharj21/assets/54074505/3749c371-8bde-44d4-b34f-99273b7c7ab8)


1. go to resource group.
2.  click on create and search for "Storage Account".
3.  create storage account and give all the details like global name etc.
4.  in the advanaced section there is a option to choose named as Data Lake storage Gen2 or hierarchical namespace. we are going to use data lake as input so check the box named as "Enable hierarchical namespace" in Data lake Gen2.This will create the data lake. if we don't check it then azure will create normal storage.
5.  Just keep all the settings as default in other sections.
6.  Create Storage account.
   
