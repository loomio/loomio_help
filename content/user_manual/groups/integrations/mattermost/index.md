---
title: Mattermost integration
description: Connecting your Loomio group notifications to your Mattermost team chat.
weight: 40
hidetoc: true
menu:
  main:
    name: Mattermost
    identifier: mattermost
    parent: integrations
---

Loomio can send notifications into your Mattermost channels when new discussions, proposals, comments, votes, and outcomes occur. Get key updates, at the right time, on important discussions and decisions.

After choosing the Mattermost channels where you want to receive notifications, and from which Loomio groups or subgroups, you will choose which kinds of events you want that channel to be notified of (comments, polls, outcomes... [see below](#select-notifications)). Read on for step-by-step instructions for integrating.

*These webhook integrations are currently in public beta testing, we would like to hear your [feedback](https://loomio.org/contact/?utm_campaign=mattermost-integration-help&utm_term=help) about how it works for your group.*

---

Start from your Mattermost team in your browser. Then open the Integrations settings page.
![](mm1.png)

Click "Incoming Webhooks"
![](mm2.png)

Then click  "Add Incoming Webhook"
![](mm3.png)

Give it a simple name, select the channel for notifications to appear within, and click Save
![](mm4.png)

Copy the Webhook URL to your clipboard, you're going to need it the next step.
![](mm5.png)

Visit your Loomio group Settings page, then click Webhooks, then Add Webhook.
![](mm6.png)

Select "Markdown (For Mattermost..)", give it a name, paste your URL from above, and click Save.
![](mm7.png)

## Select notifications

Along with the ability to choose which events in Loomio will create a post in your chosen channel, you can also choose whether you'd like a snippet of the text from the comment, proposal, outcome, etc. by using the first option.

![](../slack_teams_notifications_from_loomio.png)

_Loomio is not created by, affiliated with, or supported by Mattermost._
