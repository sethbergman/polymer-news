# Polymer News
------
![](https://raw.githubusercontent.com/sethbergman/polymer-news/a56cc75c004ce08c8d9dac917605fce0b5b2909a/NEWS.png)

## Setup
_Make sure you have NPM and Node.js installed._

### Install Polymer CLI

`npm install -g polymer-cli@next
`

### Install dependencies

`bower install
`

### Run application with development server

`polymer serve
`

### Build

`polymer build
`

### Deployment

I have been using [Firebase](https://firebase.google.com/docs/hosting/deploying) to host my Polymer apps. It's a very simple setup.

Once I've run the `polymer build` command, I initialize a new project in Firebase with `firebase init` and follow the prompts. I don't change the default values, except for the public directory setting.

Running `polymer build` bundles your files, and makes them accessable from the build/bundled directory. This project is configured to build in the `build/default` directory.

Then run `firebase deploy -p build/default` and viola!

Lastly, I will connect my own domain and firebase will provision an SSL on it for free. It doesn't get much simpler than that my friends!

### Resources

* __[Polymer Project](https://www.polymer-project.org/)__

* __[Webcomponents.org](https://www.webcomponents.org/)__

### Demo

__[Polymer News Demo](https://news.npmstack.com/)__
