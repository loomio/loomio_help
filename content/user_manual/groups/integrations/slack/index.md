---
title: Slack integration
description: Connect your Loomio group notifications to Slack.
weight: 10
hidetoc: true
menu:
  main:
    name: Slack
    identifier: slack
    parent: integrations
---

Integrate Loomio groups into one or more Slack channels to get key updates, at the right time, on the discussions and decisions that move your efforts forward.

Choose the Slack channels you want to receive notifications from which Loomio groups or subgroups and choose which kinds of events you want that channel to be notified of (comments, polls, outcomes... [see below](#select-notifications)).

*These webhook integrations are currently in public beta testing, we would like to hear your [feedback](https://loomio.org/contact/?utm_campaign=slack-integration-help&utm_term=help) about how it works for your group.*

---

Start by visiting [https://api.slack.com](https://api.slack.com), signing in if you are not already, then clicking Create New App

![](s1.png)

Give your Slack app a name

![](s2.png)

Add incoming webhooks support

![](s3.png)

Then enable the function

![](s4.png)

Then add a new webhook

![](s5.png)

Select a channel

![](s6.png)

Copy the webhook URL to your clipboard

![](s7.png)

Go to Webhooks in your Loomio group settings

![](s8.png)

Select Slack, give it a name, paste the URL, and save. You're done!

![](s9.png)

## Select notifications

Along with the ability to choose which events in Loomio will create a post in your chosen Slack channel, you can also choose whether you'd like a snippet of the text from the comment, proposal, outcome, etc. by using the first option.

![](../slack_teams_notifications_from_loomio.png)


_Loomio is not created by, affiliated with, or supported by Slack._
