## FlowForge Handbook

This repository contains the source for FlowForge's Company Handbook, detailing
information about how FlowForge Inc. is run.

All content for the Handbook can be found inside the [./src](./src) folder.

#### Contributing

The handbook is maintained on [GitHub](https://github.com/flowforge/handbook) and contributions can be made through pull-requests.

All changes merged to the `main` branch will be automatically deployed to the handbook on the
[FlowForge website](https://flowforge.com/handbook).

#### Private information

Whilst instinctively we want to be open in all we do, there will inevitably by content that is not appropriate
to make public. That content should, instead, be shared on the FlowForge Google Drive.

## Building the site locally

To run a local copy of the handbook you first need to clone the website and the handbook into side by side directories.

Once you have them both cloned, open a **bash** terminal in the website root directory and install the project dependencies. Then, run the website's eleventy server:

From the website directory:

```bash
npm install

npm start
```

This will run the website on http://localhost:8080, and then you can access the Handbook at http://localhost:8080/handbook. This will automatically reload whenever any content is changed.

**Note:** if you modify any of the Handbook's CSS, it may take a while for the website to recognise the changes. As a shortcut, you can run `npm run tailwind` to rebuild the CSS content.
