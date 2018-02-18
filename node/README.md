# Messenger Platform Sample -- node.js

This project is a server for Messenger Platform built in Node.js, modified from an example server. With this app, you can send it messages and it will echo them back to you. You can also see examples of the different types of Structured Messages.

It contains the following functionality:

* Webhook (specifically for Messenger Platform events)
* Send API
* Web Plugins
* Messenger Platform v1.1 features

## Setup

Set the values in `config/default.json` before running the sample. Descriptions of each parameter can be found in `app.js`. Alternatively, you can set the corresponding environment variables as defined in `app.js`.

Replace values for `APP_ID` and `PAGE_ID` in `public/index.html`.

## Run

You can start the server by running `npm start`. However, the webhook must be at a public URL that the Facebook servers can reach. Therefore, running the server locally on your machine will not work.

You can run this example on a cloud service provider like Heroku, Google Cloud Platform or AWS.

## Webhook

All webhook code is in `app.js`. It is routed to `/webhook`. This project handles callbacks for authentication, messages, delivery confirmation and postbacks. More details are available at the [reference docs](https://developers.facebook.com/docs/messenger-platform/webhook-reference).

## License

See the LICENSE file in the root directory of this source tree. Feel free to use and modify the code.
