---
title: First Worker
pcx_content_type: learning-unit
weight: 1
layout: learning-unit
---

## Build and deploy your first Worker

You can deploy your first Worker via the Cloudflare dashboard or programmatically using your terminal.

You must have a Cloudflare account to create a Worker. To get started with Cloudflare and create an account, refer to [Get started with Cloudflare](/learning-paths/get-started/).

### Via the Cloudflare dashboard

{{<render file="_get-started-dash.md" productFolder="workers">}}

### Via C3 and Wrangler

#### Prerequisites

{{<render file="_prereqs.md" productFolder="workers">}}

#### Create and deploy your first Worker

{{<render file="_c3-definition.md" productFolder="workers">}}

To create your Worker project, run:

{{<render file="_c3-run-command.md" productFolder="workers">}}

This will prompt you to install the [`create-cloudflare`](https://www.npmjs.com/package/create-cloudflare) package, and lead you through setup.

To set up a basic Worker:

1. Name your new Worker directory by specifying where you want to create your application.
2. Select `"Hello World" Worker` as the type of application you want to create.
3. Answer `yes` or `no` to using TypeScript.

{{<Aside type="note">}}

This guide assumes that you will use a JavaScript project. If you are creating a TypeScript project, the files will be `.ts`, a `.tsconfig` file will be created, and proper dependencies will be added.

{{</Aside>}}

You will be asked if you would like to deploy the project to Cloudflare.

- If you choose to deploy, you will be asked to authenticate (if not logged in already), and your project will be deployed to the Cloudflare global network and available on your custom [`workers.dev` subdomain](/workers/configuration/routing/workers-dev/).

- If you choose not to deploy, go to the newly created project directory to begin writing code. Deploy your project by running the [`wrangler deploy`](/workers/wrangler/commands/#deploy) command.

Refer to [How to run Wrangler commands](/workers/wrangler/commands/#how-to-run-wrangler-commands) to learn how to run Wrangler commands according to your package manager.

In your Worker project directory, C3 has generated the following:

1. `wrangler.toml`: Your [Wrangler](/workers/wrangler/configuration/#sample-wranglertoml-configuration) configuration file.
2. `index.js` (in `/src`): A minimal `'Hello World!'` Worker written in [ES module](/workers/reference/migrate-to-module-workers/) syntax.
3. `package.json`: A minimal Node dependencies configuration file.
4. `package-lock.json`: Refer to [`npm` documentation on `package-lock.json`](https://docs.npmjs.com/cli/v9/configuring-npm/package-lock-json).
5. `node_modules`: Refer to [`npm` documentation `node_modules`](https://docs.npmjs.com/cli/v7/configuring-npm/folders#node-modules).

To continue building your Worker, open the `index.js` file to write your code. Refer to [Examples](/workers/examples/) to use ready-made code you can experiment with.

## Video tutorial

If you prefer to follow along with a video tutorial, or have already created your first Worker but want to learn what more you can do with your project, review the following Learn Cloudflare Workers course for beginners.

In this course, you will:

- Deploy your first Worker.
- Develop your application locally.
- Add the Hono framework to your project.
- Integrate Workers AI into your project.

<div style="position: relative; padding-top: 56.25%;">
    <iframe
        src="https://customer-1mwganm1ma0xgnmj.cloudflarestream.com/7cb5528acbea8502c810781e1970b453/iframe?preload=true&letterboxColor=transparent"
        style="border: none; position: absolute; top: 0; left: 0; height: 100%; width: 100%;"
        allow="accelerometer; gyroscope; autoplay; encrypted-media; picture-in-picture;"
        allowfullscreen="true">
    </iframe>
</div>

Find [the video on YouTube](https://youtu.be/H7Qe96fqg1M?si=GVkdGLrmb1faiHma) and explore other Cloudflare Workers tutorials.
## Summary

You have learned how to:

- Create and deploy a Worker project using the Cloudflare dashboard and programmatically, using your terminal.

In the next module, you will learn more about Cloudflare Developer Platform.

### Related resources

* [Get started guide](/workers/get-started/guide/) - Create a new Worker with Cloudflare Workers' Get started guide.