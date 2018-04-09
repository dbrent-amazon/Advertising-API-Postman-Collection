
### Import the Collection

To import a collection into Postman, click the Import button.

![](https://github.com/dbrent-amazon/Advertising-API-Postman-Collection/blob/master/img/postman-import.png)

If you cloned the repository using Git, choose "Import Folder" and select the folder that you cloned. Or drag and drop, if you prefer.

![](https://github.com/dbrent-amazon/Advertising-API-Postman-Collection/blob/master/img/postman-import-folder.png)

This will import both the environment and the collection at the same time.

![](https://github.com/dbrent-amazon/Advertising-API-Postman-Collection/blob/master/img/postman-import-folder-select.png)

If you chose not to install Git or clone the repository, you will need to select "Paste Raw Text" and copy/paste both the collection and environment JSON separately.

### Checking the Environment

At this point, you should have both the collection and environment loaded into Postman. To check the environment, click the gear then click "Manage Environments" in the upper-right of Postman.

![](https://github.com/dbrent-amazon/Advertising-API-Postman-Collection/blob/master/img/manage-environments.png)

Here, you should see the newly imported "Advertising API" environment.

![](https://github.com/dbrent-amazon/Advertising-API-Postman-Collection/blob/master/img/manage-env-list.png)

Click it to expand its properties.

![](https://github.com/dbrent-amazon/Advertising-API-Postman-Collection/blob/master/img/manage-env-expand.png)

The only property you should ever need to modify is the PROFILE_ID. It is already set to one that works. The client Id and secret are set to the team development Ids. Feel free to change this to your own. If you do, you will need to generate a new REFRESH_TOKEN.

Click "Cancel" or "Update" when you are fnished. Before continuing, make sure the Advertising API is the active environment.

![](https://github.com/dbrent-amazon/Advertising-API-Postman-Collection/blob/master/img/postman-env-selected.png)

### Checking the Collection

You should see the newly imported Advertising API collection. Not all API calls have been implemented.

![](https://github.com/dbrent-amazon/Advertising-API-Postman-Collection/blob/master/img/postman-collection.png)

### Refresh the Access Token

Prior to making any API call, you must have a valid access token. Access tokens are only valid for one hour. After which, you must generate a new one. Click "getAccessToken" in the collections window.

![](https://github.com/dbrent-amazon/Advertising-API-Postman-Collection/blob/master/img/get-access-token.png)

On the right-hand side of Postman, feel free to look at the headers and other properties that make up the getAccessToken call.

You will also notice on the "Tests" tab there is some code that will automatically set the access and refresh token environment variables. This is for convenience. Code here is invoked after the call is made. You can find more details in the Postman documentation.

![](https://github.com/dbrent-amazon/Advertising-API-Postman-Collection/blob/master/img/postman-token-tests.png)

Click "Send".

![](https://github.com/dbrent-amazon/Advertising-API-Postman-Collection/blob/master/img/postman-send.png)
