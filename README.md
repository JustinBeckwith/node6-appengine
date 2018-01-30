# Node.js 6.0 -> Google App Engine

[![Greenkeeper badge](https://badges.greenkeeper.io/JustinBeckwith/node6-appengine.svg)](https://greenkeeper.io/)

This is a simple guide to running Node.js 6.0.0 on Google App Engine. 

1. [Create a new Node.js app](https://nodejs.org)

1. In your `package.json`, use the [engines] property to set the node.js version to 6.0.0:

  ```json
  "engines": {
    "node": "6.0.0"
  }
  ```

1. Create a project in the [Google Developers Console](https://console.developers.google.com/).

1. Make sure you have the [Google Cloud SDK](https://cloud.google.com/sdk/) installed. 

    ```sh
    $ curl https://sdk.cloud.google.com | bash 
    $ gcloud init
    $ gcloud components update app
    ```

1. Deploy your app:

    ```sh
    gcloud preview app deploy
    ```

You are now running Node.js 6.0 App Engine. How cool is that? 
