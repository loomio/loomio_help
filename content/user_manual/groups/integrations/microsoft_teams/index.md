---
title: Microsoft Teams integration
description: Connect your Loomio group notifications to Microsoft Teams.
weight: 30
hidetoc: true
menu:
  main:
    name: Microsoft Teams
    identifier: microsoft_teams
    parent: integrations
---

Loomio can send notifications into your Microsoft Teams when new discussions, proposals, comments, votes, and outcomes occur. Get key updates, at the right time, on important discussions and decisions.

After choosing where you want to receive notifications in Teams, and from which Loomio groups or subgroups, you will choose which kinds of events you want that channel to be notified of (comments, polls, outcomes... [see below](#select-notifications)). Read on for step-by-step instructions for integrating.

*These webhook integrations are currently in public beta testing, we would like to hear your [feedback](https://loomio.org/contact/?utm_campaign=teams-integration-help&utm_term=help) about how it works for your group.*

---

Visit [https://teams.microsoft.com](https://teams.microsoft.com) then click Apps
![](t1.png)

Search for "webhook" in the search field, then click Incoming Webhook
![](t2.png)

Click "Add to a team"
![](t3.png)

Type and select the channel you want Loomio notifications to appear within.
![](t4.png)

Give it a name, such as "Loomio notifications", then click "Create"
![](t5.png)

Copy the URL it gives you, you'll paste it into Loomio in the last step.
![](t6.png)

Go to your Loomio group Settings then click Webhooks
![](t7.png)

Select Microsoft Teams, give it a name, paste the URL, and click Save.
![](t8.png)

## Select notifications

Along with the ability to choose which events in Loomio will create a post in your chosen channel, you can also choose whether you'd like a snippet of the text from the comment, proposal, outcome, etc. by using the first option.

![](../slack_teams_notifications_from_loomio.png)

_Loomio is not created by, affiliated with, or supported by Microsoft._
