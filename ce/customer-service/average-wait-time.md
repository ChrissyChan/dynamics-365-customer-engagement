---
title: "Show customers their average wait time in a queue | MicrosoftDocs"
description: "How to show customers their average wait time for a chat widget in Omnichannel for Customer Service."
author: lalexms
ms.author: laalexan
manager: shujoshi
ms.date: 05/07/2021
ms.topic: article
ms.service: dynamics-365-customerservice
---

# Show customers their average wait time in a queue


[!INCLUDE[cc-use-with-omnichannel](../includes/cc-use-with-omnichannel.md)]

## Overview

As an administrator, you can enable the feature that displays a customer's average wait time in the queue when they're waiting to chat with an agent. It helps set customer expectations when wait times are long because of a high volume of customers needing support, understaffing, or long call-handling times. When you display the average wait time to the customer, the customer can decide whether to wait in the queue or return to the chat later.

With this feature turned on, when a new customer is placed in the queue, they are notified with the following message: **Average wait time \<n\> mins.** The average wait time is displayed only if the wait is one minute or longer.

The average wait time is calculated based on wait times from the previous 48 hours and a minimum of 50 conversations for the specific queue. This is an estimated time, and doesn't change for the customer. When there is no wait, the average wait time isn't displayed.

> [!NOTE]
> If skill-based routing is configured with exact skill match, the queue position that's displayed to a customer on the chat portal widget might not be accurate; therefore, the assignment of an agent to the customer might take longer than expected.

## Enable average wait time

If you're using Omnichannel admin center, do the following:

1. Go to the workstream of the chat widget in which you need to configure the settings, select edit for the required chat widget, and on the **Chat channel Settings** page, go to the **Behaviors** tab.
2. Select **Show average wait time** if you want to show to customers the average wait time in the queue when they're waiting to interact with an agent.
3. Save and close.

If you're using Omnichannel Administration, do the following:

1. Go to **Channels** &gt; **Chat**, and open the chat widget in which you need to configure the settings.
2. Select the **General settings** tab.
3. In the **Customer waiting** area, change **Show average wait time** to **Yes**. By default, it is set to **No**.
4. Select **Save**.

### See also

[Show customers their position in a queue](show-queue.md) <br>
[Overview of skill-based routing](overview-skill-work-distribution.md) <br>
[Add a chat widget](add-chat-widget.md) <br>
[Configure a pre-chat survey](configure-pre-chat-survey.md) <br>
[Configure agent display name](agent-display-name.md)<br>
[Create quick replies](create-quick-replies.md) <br>
[Create and manage operating hours](create-operating-hours.md) <br>
[Create chat authentication settings](create-chat-auth-settings.md) <br>
[Embed chat widget in Power Apps portals](embed-chat-widget-portal.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
