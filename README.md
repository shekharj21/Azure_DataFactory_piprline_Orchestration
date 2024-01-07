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
   
## Deploy Azure Data Factory :
![Screenshot (488)](https://github.com/shekharj21/shekharj21/assets/54074505/9f7ae069-9dff-4633-8633-38bddeca7274)

1. Search data Factories in add resource in home tab.
2. select reosurce group, naame and region.
3. keep all other section settings as default and select create.

## Deploy Azure SQL DB :

![Screenshot (489)](https://github.com/shekharj21/shekharj21/assets/54074505/1335e164-d4f5-4b6a-b663-d2d7587c94b2)

1. Find Azure SQL DB.
2. add resouce group, DB name. we don't have server so there is a option "create new" under Server. Click it.
3. Give all the detailsa and choose SQL authentication and create server.
4. After that Go to "compute + storage" and choose the bare minimum plan FOR COST SAVING.
5. Keep all other section setting as default.
6. Create a SQL DB.
7. after creaing Db, go to the Db and choose set firewall access and add your own IPv4 Address.
8. go and then check qurey editior (access on the left section of DB).
