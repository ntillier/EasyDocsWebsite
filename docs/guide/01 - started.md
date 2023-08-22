---
slug: 'getting-started'
label: 'Getting started'
---


# Getting Started
The onboarding process for EasyDocs is incredibly swift and user-friendly—simply ensure that you have Node.js installed.

# Installing EasyDocs
Begin by installing EasyDocs globally:

```bash
npm install @nathanti/easydocs --global
```

!!! hint Update EasyDocs
Keeping EasyDocs up to date is as straightforward as its installation:
```bash
npm update @nathanti/easydocs --global
```
!!!

# Creating a Project
In your terminal, execute the following command to generate a new directory:
```bash
mkdir easydocs-test
```

Navigate to this directory:
```bash
cd ./easydocs-test
```

Then, run this command to initiate the project setup, configuring the requisite folders and files:

```bash
easydocs init
```

Now, within the project directory using a file explorer, you will notice the presence of specific folders and files:

* `/docs`: This folder houses the markdown files for documentation.
* `/public`: This is where you can store images and other public assets.
* `/docs.config.json`: This file serves as the project's configuration.

# Running Your Project
Execute the following command to run your project:
```bash
easydocs dev
```

At this point, you can preview the website in your preferred browser.

!!! info Development Mode
Running this command initiates EasyDocs in development mode, enabling automatic parsing of modified content within the `/docs` folder. Refreshing the browser tab will reveal the updated version.
!!!

# Serving Your Project
Use this command to serve your project:
```bash
easydocs serve
```
Similar to easydocs dev, this command operates without actively monitoring changes within the /docs directory.

# Building Your Project
Execute the following command to build your project:
```bash
easydocs build
```
This will compile your project and generate a `/.build` directory containing all the necessary files. You can then proceed to publish it on GitHub Pages or your preferred hosting platform.