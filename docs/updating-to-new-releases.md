---
id: updating-to-new-releases
title: Updating to New Releases
---

Create React SSR App is divided into two packages:

- `create-react-ssr-app` is a global command-line utility that you use to create new projects.
- `react-ssr-scripts` is a dependency in the generated projects (including this one).

You almost never need to update `create-react-ssr-app` itself: it delegates all the setup to `react-ssr-scripts`.

When you run `create-react-ssr-app`, it always creates the project with the latest version of `react-ssr-scripts` so you’ll get all the new features and improvements in newly created apps automatically.

To update an existing project to a new version of `react-ssr-scripts`, [open the changelog](https://github.com/trustworktech/create-react-ssr-app/blob/master/CHANGELOG.md), find the version you’re currently on (check `package.json` in this folder if you’re not sure), and apply the migration instructions for the newer versions.

In most cases bumping the `react-ssr-scripts` version in `package.json` and running `npm install` (or `yarn install`) in this folder should be enough, but it’s good to consult the [changelog](https://github.com/trustwoktech/create-react-ssr-app/blob/master/CHANGELOG.md) for potential breaking changes.

We commit to keeping the breaking changes minimal so you can upgrade `react-ssr-scripts` painlessly.
