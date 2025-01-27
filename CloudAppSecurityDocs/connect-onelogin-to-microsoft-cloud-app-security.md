---
title: Connect OneLogin to Cloud App Security
description: This article provides instructions for connecting Microsoft Cloud App Security to your existing OneLogin app using the App Connector APIs. 
ms.date: 06/09/2021
ms.topic: how-to
---
# Connect OneLogin to Microsoft Cloud App Security

[!INCLUDE [Banner for top of topics](includes/banner.md)]

This article provides instructions for connecting Microsoft Cloud App Security to your existing OneLogin app using the App Connector APIs. This connection gives you visibility into and control over your organization’s OneLogin use.

## Prerequisites

- The OneLogin account used for logging into OneLogin must be a Super User. For more information about OneLogin administrative privileges, see [this article](https://onelogin.service-now.com/kb_view_customer.do?sysparm_article=KB0010391).

## How to connect OneLogin to Cloud App Security

### Configure OneLogin

1. Go to the OneLogin admin portal. Select **API Credentials** in the **Developers** dropdown menu.

    ![Select API credentials](media/api-credentials-onelogin.png)

1. Select **New Credential**.
1. Name your new application as **Microsoft Cloud App Security**, choose **Read all** permissions, and select **Save**.

    ![Create new API credential](media/create-new-api-credential-onelogin.png)

1. Copy the **Client ID** and the **Client Secret**. You'll need them in the following steps.

### Configure Cloud App Security

1. In the [Cloud App Security portal](https://portal.cloudappsecurity.com/), select **Investigate** and then **Connected apps**.
1. In the **App connectors** page, select the plus button followed by **OneLogin**.
1. In the pop-up, give the connector a descriptive name, and select **Connect OneLogin**.

    ![Connect OneLogin](media/connect-onelogin.png)

1. Enter the **Client ID** and the **Client Secret** that you copied and select **Connect OneLogin**.
1. Make sure the connection succeeded by selecting Test now. Testing may take a couple of minutes. After receiving a success notice, select **Close**.
1. The first connection can take up to 4 hours to get all users and their activities after the connector was established.
1. After the connector’s **Status** is marked as **Connected**, the connector is live and working.

## Next steps

> [!div class="nextstepaction"]
> [Control cloud apps with policies](control-cloud-apps-with-policies.md)

[!INCLUDE [Open support ticket](includes/support.md)]
