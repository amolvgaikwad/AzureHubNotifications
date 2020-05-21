# AzureHubNotifications
Integration of azure cloud messaging center to receive the notifications &amp; Azure Rest API's &amp; Method Integration to send the notification.  

Please refer below steps for How to broadcast azure notification from your application.

1. Add AzureNotificationRestApi package in your PCL solution. 
2. Use below apis

    APIManager.SingletonInstance.SetAzureConfigurations("Access Endpoint","NameSpace","Hub Name");
    await APIManager.SingletonInstance.SendNotificationWithTags("Notification Description","TagName",PlatformEnum.All);

Thats all you need to do to enable serverless notification functioanlity.  

 
