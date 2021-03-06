# How to register a V1 Web application

This tutorial introduces how to register the application using Microsoft Azure portal.
Once you registered an application by following this tutorial, you can use it as a "Web app / API" in Office365APIEditor.

1. Go to https://portal.azure.com/ and sign in using your administrator account of Microsoft Azure.

2. Click [Azure Active Directory] in the left panel.

3. Click [App registration] tab.

4. Click [New application registration].

5. Enter the name of your application. (e.g. MyWebApp)

6. Select [Web app / API].

7. Enter the sing-on URL of your application in [Sign-on URL] box. (e.g. https&#58;<span></span>//localhost/MyWebApp <- Whatever is fine.)

8. Click [Create].

9. Click the application which you created.

10. Click [Keys].

11. Enter the name of your key. (e.g. Key01)

12. Select the duration of the key. (e.g. 2 years)

13. Click [Save].

14. Copy the [Value] to the safety place.

15. Click [Required permissions] and add the necessary permissions for your application.
If your application has to read the messages in users mailbox using Office 365 API (outlook.office.com), you have to add the [Read user mail] permission under [DELEGATED PERMISSIONS] of [Office 365 Exchange Online (Microsoft.Exchange)].
If your application has to read the messages in users mailbox using Graph API (graph.microsoft.com), you have to add the [Read user mail] permission under [DELEGATED PERMISSIONS] of [Microsoft Graph].

16. Check the following values and use them in Office365APIEditor.

  | Value in Azure portal | Textbox in Office365APIEditor |  
  |:----------------------|-------------------------------|  
  |Application ID         |Application ID                 |  
  |Reply URL              |Reply URL                      |  
  |Value of Key           |Key                            |  
