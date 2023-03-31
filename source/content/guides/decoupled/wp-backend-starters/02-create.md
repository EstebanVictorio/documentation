---
title: Decoupled WordPress Backend Starter for Front-End Sites
subtitle: Create a New Project
description: Learn how to create a new decoupled WordPress backend project.
tags: [webops, workflow, decoupled]
contributors: [backlineint, cobypear, hckia, whitneymeredith]
layout: guide
showtoc: true
permalink: docs/guides/decoupled/wp-backend-starters/create
anchorid: create
contenttype: [guide]
innav: [true]
categories: [create]
cms: [decoupled]
audience: [development]
product: [decoupled]
integration: [--]
---

This section provides information on how to create a new WordPress backend project with Pantheon's starter kit.

### Install with Dashboard Upstream

1. Log in to your Pantheon Dashboard and select the **Sites** page.

1. Click the **Front-End Sites** tab and then click **+Create New Site**.

1. Select **Front-End Site**, and then select **WordPress for Front-End** under **Create Backend CMS**.

    - You can also use the [Decoupled WordPress Composer Managed](https://dashboard.pantheon.io/sites/create?upstream_id=c9f5e5c0-248f-4205-b63a-d2729572dd1f) link to create your site in the Pantheon Dashboard.

    ![select a starter](../../../../images/decoupled-select-starter.png)

1. Name your site, select your decoupled environment from the **Choose a Workspace for the Site** drop-down menu, and then click **Continue**. You cannot use a . (period) or _ (underscore) for site and Multidev names.

1. Confirm your organization selection when prompted in the **Confirm Organization Selection** dialogue box. The Deploying Decoupled WordPress Composer Managed progress indicator displays while your site is spinning up.

1. Click **Visit your Pantheon Dashboard** when the site spin up completes.

1. Click the **Visit Development Site** button to install WordPress.

1. Select the profile. This can also be done via
[`terminus remote:wp`](/terminus/commands/remote-wp).

Your backend starter is ready to develop!

Note that you can also use Terminus to initiate the site spin up in the Pantheon Dashboard:

Run the command below in Terminus:

```bash{promptUser: user}
 terminus site:create my-new-site "Describe Site" --org='My Team Name' c9f5e5c0-248f-4205-b63a-d2729572dd1f
```

<Alert title="Note"  type="info" >

  - Replace `{My Team Name}` with your team name - for example `My Agency`. This can also be omitted.
  - `c9f5e5c0-248f-4205-b63a-d2729572dd1f` is the `upstream_id` for Decoupled WordPress Composer Managed.

</Alert>