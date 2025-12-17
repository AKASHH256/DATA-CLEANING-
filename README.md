# Overview

> Share your Replit Apps with the world in just a few clicks.

export const YouTubeEmbed = ({videoId, title = "YouTube video", startAt}) => {
  if (!videoId) {
    return null;
  }
  let url = "https://www.youtube.com/embed/" + videoId;
  if (startAt) {
    url = url + "?start=" + startAt;
  }
  return <Frame>
      <iframe src={url} title={title} allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowFullScreen></iframe>
    </Frame>;
};

Publishing lets you share your Replit App with the world using a simplified process.

<Note>
  The action of making your app live is called "Publishing." This page describes the different types of deployments available.
</Note>

## What is Publishing?

Publishing is a feature that saves a **snapshot** of your Replit App to the cloud,
where everyone can interact with it. A snapshot captures the current state of the files in your
Replit App.

When you publish your Replit App, you create a **published app**. A published app is a running instance
of your app on Replit's cloud infrastructure. This makes the app reliably available on the internet,
separate from the version in your workspace.

<Info>
  Replit's infrastructure is backed by Google Cloud Platform (GCP). All
  published apps are hosted in the United States.
</Info>

Publishing includes tools to monitor your published app status and view web analytics.

Replit offers the following deployment types:

<CardGroup>
  <Card title="Autoscale Deployment" href="/cloud-services/deployments/autoscale-deployments" icon="layer-group">
    Automatically adjusts resources based on your app's usage.
  </Card>

  <Card title="Static Deployment" href="/cloud-services/deployments/static-deployments" icon="files">
    Provides an affordable way to host websites that don't change based on user input.
  </Card>

  <Card title="Reserved VM Deployment" href="/cloud-services/deployments/reserved-vm-deployments" icon="server">
    Provides a consistent amount of computing resources for your app to run continuously.
  </Card>

  <Card title="Scheduled Deployment" href="/cloud-services/deployments/scheduled-deployments" icon="clock">
    Runs your app at scheduled times that you choose.
  </Card>
</CardGroup>

## Getting started

Follow the steps below to publish your Replit App:

1. From your Replit App workspace, select <img class="icon-svg" src="https://mintcdn.com/replit/rBzGsKp9NcWJ7sib/images/icons/deploy-icon.svg?fit=max&auto=format&n=rBzGsKp9NcWJ7sib&q=85&s=df3fa2573b451c54591523c9d9111db1" alt="Publish icon" data-og-width="16" width="16" data-og-height="16" height="16" data-path="images/icons/deploy-icon.svg" data-optimize="true" data-opv="3" srcset="https://mintcdn.com/replit/rBzGsKp9NcWJ7sib/images/icons/deploy-icon.svg?w=280&fit=max&auto=format&n=rBzGsKp9NcWJ7sib&q=85&s=115e9383e0350a6ef201a41f78f8a19a 280w, https://mintcdn.com/replit/rBzGsKp9NcWJ7sib/images/icons/deploy-icon.svg?w=560&fit=max&auto=format&n=rBzGsKp9NcWJ7sib&q=85&s=667b93ae66d0b69569409fb90d9fc280 560w, https://mintcdn.com/replit/rBzGsKp9NcWJ7sib/images/icons/deploy-icon.svg?w=840&fit=max&auto=format&n=rBzGsKp9NcWJ7sib&q=85&s=ae927e5aadcb7a470ad726f0acb0f782 840w, https://mintcdn.com/replit/rBzGsKp9NcWJ7sib/images/icons/deploy-icon.svg?w=1100&fit=max&auto=format&n=rBzGsKp9NcWJ7sib&q=85&s=16ee8f7b3d9db6b4f74ea8c2ebb6730f 1100w, https://mintcdn.com/replit/rBzGsKp9NcWJ7sib/images/icons/deploy-icon.svg?w=1650&fit=max&auto=format&n=rBzGsKp9NcWJ7sib&q=85&s=ad04a5984543c13895fd30182294ec0a 1650w, https://mintcdn.com/replit/rBzGsKp9NcWJ7sib/images/icons/deploy-icon.svg?w=2500&fit=max&auto=format&n=rBzGsKp9NcWJ7sib&q=85&s=2449268bce371256727b17027eb180f3 2500w" /> **Publish** at the top.
2. In the **Publishing** tab, select your publishing option.
3. If **Add a payment method** appears, follow the prompts to add a payment method.

Replit automatically selects the best publishing option for your app based on the project type and your needs.

However, to choose a different deployment type, consider the following information.

## Choosing the right publishing option

The following video explains how to choose the right publishing option for your app:

<YouTubeEmbed videoId="OqSbgBMoTm0" />

Use the following decision tree featured in the video to help you choose:

<Frame>
  <img src="https://mintcdn.com/replit/jSmYU1wBTvl8UMyc/images/deployments/decision-tree.png?fit=max&auto=format&n=jSmYU1wBTvl8UMyc&q=85&s=8129fe2205ca99224ea9a3707072bcf9" data-og-width="5344" width="5344" data-og-height="6250" height="6250" data-path="images/deployments/decision-tree.png" data-optimize="true" data-opv="3" srcset="https://mintcdn.com/replit/jSmYU1wBTvl8UMyc/images/deployments/decision-tree.png?w=280&fit=max&auto=format&n=jSmYU1wBTvl8UMyc&q=85&s=04a6a7b9b41cc95d9a82ea04bbcb75ff 280w, https://mintcdn.com/replit/jSmYU1wBTvl8UMyc/images/deployments/decision-tree.png?w=560&fit=max&auto=format&n=jSmYU1wBTvl8UMyc&q=85&s=78e45134e452cd4fbfed83b24cf3b94a 560w, https://mintcdn.com/replit/jSmYU1wBTvl8UMyc/images/deployments/decision-tree.png?w=840&fit=max&auto=format&n=jSmYU1wBTvl8UMyc&q=85&s=10f8cc59f1b608e869a971140f455727 840w, https://mintcdn.com/replit/jSmYU1wBTvl8UMyc/images/deployments/decision-tree.png?w=1100&fit=max&auto=format&n=jSmYU1wBTvl8UMyc&q=85&s=85a3a3d3f96e363958fe41c517e2b18a 1100w, https://mintcdn.com/replit/jSmYU1wBTvl8UMyc/images/deployments/decision-tree.png?w=1650&fit=max&auto=format&n=jSmYU1wBTvl8UMyc&q=85&s=bb9f224be7530ecd7b8bdfe4ee372129 1650w, https://mintcdn.com/replit/jSmYU1wBTvl8UMyc/images/deployments/decision-tree.png?w=2500&fit=max&auto=format&n=jSmYU1wBTvl8UMyc&q=85&s=901da1201a53d83241f16edf018f66ac 2500w" />
</Frame>

## Key features

Publishing offers the following convenient features:

* **Multiple publishing options**: Select or update a deployment type that meets your needs in a few clicks.
* **Custom domains**: Serve your app from your web domain.
* **Analytics**: Track visitor data and other metrics for your published app.
* **Monitoring tools**: View your published app status and configuration.
* **Access controls**: Control who can see your app with a single click. Available only for **Teams** members.

## How it works

When you publish your Replit App, Replit creates a snapshot of your app's files and dependencies.
This snapshot is then sent to Replit's cloud infrastructure, where it runs as a separate instance of your app.
To update your published app with the latest changes, publish again to create a fresh snapshot.

<Warning>
  Avoid saving and relying on data written to a published app's filesystem. To
  store data, use a storage or database option such as Replit's [Storage and
  Database](/category/storage-and-databases) offerings.
</Warning>

## Use cases

The following examples show different types of published apps.

### Autoscale deployment: Typing speed assessment app

Let the cloud scale up resources when users take typing tests and reduce them when not in use.

### Static deployment: Solar system simulation

Learn about the planets in a solar system visualization app on the web.
This visualization renders in the browser and doesn't transfer any user input to a server.

### Reserved VM deployment: Discord bot

Run a Discord bot that helps you moderate and onboard members.
It's always online to chat with users and respond to commands with predictable pricing and performance.

### Scheduled deployment: Home automation triggers

Schedule API calls to start and stop your smart home devices at specific times and days.

## Next steps

To learn more about Replit Publishing, see the following resources:

* [Autoscale Deployment](/cloud-services/deployments/autoscale-deployments/): Learn how to set up applications that scale with traffic
* [Static Deployment](/cloud-services/deployments/static-deployments/): Discover how to publish static websites quickly and efficiently
* [Reserved VM Deployment](/cloud-services/deployments/reserved-vm-deployments/): Explore dedicated VM options for specialized use cases
* [Scheduled Deployment](/cloud-services/deployments/scheduled-deployments/): Set up recurring tasks with simple scheduling
* [Custom Domains](/cloud-services/deployments/custom-domains/): Connect your published app to a custom domain


---

> To find navigation and other pages in this documentation, fetch the llms.txt file at: https://docs.replit.com/llms.txt
