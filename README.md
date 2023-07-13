# az-func-b-etl
Change the Excel format of power consumption data to CSV format and store the output on Azure Blob Storage.
# How to use
1. Clone the code from **https://github.com/asad-shmoghadam/az-func-b-etl.git**.
2. In VSCode, choose **create function** and then **choose Create new project** in the Workspace (local).
3. Choose the directory for your project.
4. Select a language and its version for your project (I used Python 3.10.9).
5. Select **Azure Blob Storage trigger**.
6. Provide a function name.
7. Create new local app setting.
8. Choose **ccpsattachmentsstorage** account.
9. Provide **attachments/{name}.xls** path.
10. Modify the function that you cloned based on your requirements.
11. Create a new Azure Function App. (You can create manually on Azure or from VSCode.)
12. Deploy your function directly from VSCode to Azure.
13. Create a container called `**powerdata**` in the **ccpsattachmentsstorage** storage account.
14. Add Azure Storage Account connection string for the atachments container to function configuration with the name of **ccpsattachmentsstorage_STORAGE.**
> The function will be triggered if the EXCEL file added to this path "path": "attachments/{name}.xls", 
