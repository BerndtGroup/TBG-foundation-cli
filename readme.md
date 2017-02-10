# TBG Foundation CLI

This is a fork of the command-line interface for [Foundation](http://foundation.zurb.com) family of frameworks for use with internal TBG projects. It downloads and installs blank templates in any of the three Foundation frameworks:

- [Foundation for Sites](http://foundation.zurb.com/sites), a framework for responsive websites.
- [Foundation for Apps](http://foundation.zurb.com/apps), a framework for responsive web apps.
- [Foundation for Emails](http://foundation.zurb.com/emails), a framework for responsive email.

## Requirements

You'll need the following software installed to get started.

  * [Node.js](http://nodejs.org) 0.12+: Use the installer provided on the NodeJS website.
    * With Node installed, run `[sudo] npm install -g gulp bower`.
  * [Git](http://git-scm.com/downloads): Use the installer for your OS.
    * Windows users can also try [Git for Windows](http://git-for-windows.github.io/).

## Installing

The Foundation CLI is installed through npm.

```bash
npm install -g tbg-foundation-cli
```

This will add the `tbg-foundation` command to your system.

### Updating

The CLI periodically gets updates that add features or fix bugs. Use npm to upgrade the CLI to the newest version.

```bash
npm update -g tbg-foundation-cli
```

To check what version you currently have, use `-v`.

```bash
tbg-foundation -v
```

## Commands

### New

Starts the setup process for a new Foundation project. The CLI will ask you which framework you want to use and a folder name for the project.

```bash
tbg-foundation new
```

### Watch

While inside of your app's folder, use the `watch` command to assemble your app and run a test server.

```bash
cd appName
tbg-foundation watch
```

While this process is running, you can view the assembled app in your browser, at this URL:

```
http://localhost:8080
```

While the server is running, any changes you make to your HTML, Sass, or JavaScript will automatically be processed and added to your live app.

### Build

To build your app for production, use `foundation build`.

```bash
tbg-foundation build
```

### Update

Updates your Bower packages, which includes Foundation. Run this command when you want to update an existing project to the newest version of Foundation.

```bash
tbg-foundation update
```

### Help

Lists all available commands in the CLI.

```bash
tbg-foundation help
```

Add a command name at the end to learn how a specific command works.

```bash
tbg-foundation help new
```
