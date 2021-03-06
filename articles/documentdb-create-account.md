<properties title="How to Create a DocumentDB Account" pageTitle="How to Create a DocumentDB Account | Azure" description="required" metaKeywords="" services="" solutions="" documentationCenter="" authors="" videoId="" scriptId="" />

<tags ms.service="documentdb" ms.workload="big-data" ms.tgt_pltfrm="na" ms.devlang="na" ms.topic="article" ms.date="01/01/1900" ms.author="" />

#How to Create a DocumentDB Account
To use DocumentDB, you must create a DocumentDB account in an available geographic region.  This topic describes how to create a DocumentDB account in the Azure management preview portal.  

##Table of Contents
-	[How to: Create a DocumentDB account][]
-	[Next steps][]
##<a id="Howto"></a>How to: Create a DocumentDB account
1.	Sign in to the Azure management preview portal
2.	Click New, DocumentDB Account.  
	![][1]  

	Alternatively, you can browse the Azure Gallery, select the “Data, storage, + backup” category, choose **DocumentDB Account** and then click **Create**.  

	![][2]  

	In the **New DocumentDB (Preview)** blade, specify the desired configuration for the DocumentDB account. 
 
	![][3] 

	In **Name**, enter a name to use in the URI for the DocumentDB account.  This value becomes the host name within the URI that is used to address the DocumentDB account.  The name entry must be a string between %/% and %/% characters, containing only %/%, and must start with %/% 

	*Note that documents.azure.com will be appended to the endpoint name you choose, the result of which will become your DocumentDB account endpoint.*

	The **Pricing Tier** lens is locked, as the DocumentDB preview supports a single standard pricing tier.

	*For more information, see the [DocumentDB pricing details](http://go.microsoft.com/fwlink/?LinkID=402317&clcid=0x409)*

	The **Optional configuration** lens is used to specify the initial capacity allocated to your DocumentDB account.  DocumentDB leverages capacity units to allow you to scale your DocumentDB account, where each capacity unit includes reserved database storage and throughput.  By default, 1 capacity unit is provisioned.  You can adjust the number of capacity units available to your DocumentDB account at any time via the [Azure management preview portal](https://portal.azure.com/).

	*For details about DocumentDB account capacity and throughput, see [Scaling with Microsoft Azure DocumentDB](about:blank).*

	In **Resource group**, select or create a resource group for your DocumentDB account.  By default, a new Resource group will be created.  You may, however, choose to select an existing resource group to which you would like to add your DocumentDB account.

	*For more information see, [Using Resource groups to manage your Azure resources](http://azure.microsoft.com/en-us/documentation/articles/azure-preview-portal-using-resource-groups/).*

	For **Subscription**, select the Azure subscription that you want to use for the DocumentDB account.

	*If your account has only one subscription, it will be automatically selected.*
 
	Use **Location** to specify the geographic location in which your DocumentDB account will be hosted. 

3.	Once the new DocumentDB account options are configured, click **Create**.  It can take a few minutes for the DocumentDB account to be created.  To check the status, you can monitor the progress on the startboard.  
	![][4]  
  
	Or from the Notifications hub.  

	![][5]  

	![][6]

4.	After the DocumentDB account has been created, it is ready for use with the default settings.

	*Note that the default consistency of the DocumentDB account will be set to Session.  You can adjust the default consistency setting via the [Azure management preview portal](https://portal.azure.com/).  For more information on DocumentDB consistency settings, see [this](http://tbd/).*  
	![][7]  

5.	You may also access your existing DocumentDB accounts from the **Browse** blade.  
	![][8]

##<a id="NextSteps"></a>Next steps
-	Learn how to [manage your DocumentDB account](about:blank).
-	To learn more about DocumentDB, see the Azure DocumentDB documentation on [azure.com](http://go.microsoft.com/fwlink/?LinkID=402319&clcid=0x409)

[How to: Create a DocumentDB account]: #Howto
[Next steps]: #NextSteps


<!--Image references-->
[1]: ./media/documentdb-create-account/ca1.png
[2]: ./media/documentdb-create-account/ca2.png
[3]: ./media/documentdb-create-account/ca3.png
[4]: ./media/documentdb-create-account/ca4.png
[5]: ./media/documentdb-create-account/ca5.png
[6]: ./media/documentdb-create-account/ca6.png
[7]: ./media/documentdb-create-account/ca7.png
[8]: ./media/documentdb-create-account/ca8.png
