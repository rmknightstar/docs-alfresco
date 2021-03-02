---
author: [Alfresco Documentation, Alfresco Documentation]
audience: 
category: Alfresco Team
option: [fileservers, CIFS, FTP]
---

# Managing file servers

The Fileservers page handles the properties for the CIFS and FTP servers.

1.  Open the Admin Console, and then click **Fileservers**.

2.  On the Fileservers page, click **Edit**.

    You see the Edit: Fileservers page. The page is divided up into sections for Filesystem properties, CIFS properties, and FTP properties.

3.  Set the Filesystem property:

    |Filesystem property|Example setting|What is it?|
    |-------------------|---------------|-----------|
    |**Filesystem Name**|Alfresco|This is the name given to the file system when using CIFS, WebDAV, or FTP. For example, Alfresco.|

4.  Set the CIFS properties for connecting to Alfresco using CIFS:

    |CIFS property|Example setting|What is it?|
    |-------------|---------------|-----------|
    |**CIFS Enabled**|enabled|This checkbox enables or disables the CIFS server.|
    |**Host Announce**|enabled|This checkbox enables the announcement of the CIFS server to the local domain/workgroup so that it shows up in Network Places/Network Neighborhood.|
    |**Domain**| |This is the domain or workgroup to which the server belongs. This defaults to the domain/workgroup of the server, if not specified.|
    |**Server Name**|$\{localname\}A|This is the host name for the Alfresco CIFS server. This can be a maximum of 16 characters and must be unique on the network. You can use the special token \{localname\} in place of the local server's host name and a unique name can be generated by prepending/ appending to it.|
    |**Session Timeout**|900|This is the CIFS session timeout value in seconds. The default session timeout is 15 minutes. If no I/O occurs on the session within this time then the session will be closed by the server. Windows clients send keep-alive requests, usually within 15 minutes.|

5.  Set the FTP properties for connecting to Alfresco using FTP:

    |FTP property|Example setting|What is it?|
    |------------|---------------|-----------|
    |**FTP Enabled**|Enabled|This checkbox enables or disables the FTP server.|
    |**Port**|2121|This is the port that the FTP server listens for incoming connections on.|
    |**Dataport From**|0|This sets the lower limit for the data ports range of ports.|
    |**Dataport To**|0|This sets the upper limit for the data ports range of ports.|

6.  Click **Save**.

    If you do not want to save the changes, click **Cancel**.


**Parent topic:**[Managing Alfresco using the Admin Console](../concepts/at-adminconsole.md)
