# loopback-angular-admin

**This software is not ready for production! It is still being developed and it will change in the future.**

The goal is to have a starter project which can be used to quickly build an API with a frontend that are easily extended.

[![Gitter](https://badges.gitter.im/Join Chat.svg)](https://gitter.im/beeman/loopback-angular-admin?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

[![NPM version](https://badge.fury.io/js/loopback-angular-admin.png)](http://badge.fury.io/js/loopback-angular-admin)
[![Dependencies](https://david-dm.org/beeman/loopback-angular-admin.png)](https://david-dm.org/beeman/loopback-angular-admin)

[![Codeship Status for beeman/loopback-angular-admin](https://www.codeship.io/projects/63461bc0-396b-0132-3ad7-621226feddc2/status)](https://www.codeship.io/projects/42207)

[![wercker status](https://app.wercker.com/status/d5bf1a6b787b3c00633c02da0f9a48e5/s "wercker status")](https://app.wercker.com/project/bykey/d5bf1a6b787b3c00633c02da0f9a48e5)

[![Build Status](https://drone.io/github.com/beeman/loopback-angular-admin/status.png)](https://drone.io/github.com/beeman/loopback-angular-admin/latest)

## Try it now!

Deploy an instance on your Heroku account to play around with it!

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

- **Guest Sign-In**: Email ```user@user.com``` Password ```user```
- **Admin Sign-In**: Email ```admin@admin.com``` Password ```admin```

## Features and implemented projects

- A Loopback REST API with authentication enabled built on the [Loopback Generator](https://www.npmjs.org/package/generator-loopback)
- A GUI built with AngularJS based on the [Angular Generator](https://github.com/yeoman/generator-angular)
- Angular UI-Router
- JSON-based based forms by [angular-formly](https://github.com/nimbly/angular-formly)
- Notifications by [angular-toasty](https://github.com/Salakar/angular-toasty)
- File upload with [Loopback storage services](https://github.com/strongloop/loopback-component-storage/)
- Admin template powered by [almasaeed2010/AdminLTE](https://github.com/almasaeed2010/AdminLTE)
- Markdown Editor with live preview with [angular-markdown-editor](https://github.com/JimLiu/angular-markdown-editor)
- Bunch of useful filters for AngularJS: [a8m/angular-filter](https://github.com/a8m/angular-filter)
- [t4t5/sweetalert](https://github.com/t4t5/sweetalert) provided by [oitozero/ngSweetAlert](https://github.com/oitozero/ngSweetAlert)
- Automatically growing textarea's by [monospaced/angular-elastic](https://github.com/monospaced/angular-elastic)
- Social authentication with [Loopback passport](https://github.com/strongloop/loopback-component-passport/)
- Multi-language support by [rubenv/angular-gettext](https://github.com/rubenv/angular-gettext)
- User management


## TODO:

- Permissions on user actions (non-admins cannot access advanced functions)
- permissions on content items (non-admins can only edit own content, etc)
- Detect if API is online [HubSpot/offline](https://github.com/HubSpot/offline)?
- Loading indicators [Urigo/angular-spinkit](https://github.com/Urigo/angular-spinkit)?
- Map API roles to [Narzerus/angular-permission](https://github.com/Narzerus/angular-permission)
- Add tests
- Add Dockerfile
- Add Vagrantfile


[Tell me what we need more!](https://github.com/beeman/loopback-angular-admin/issues/new)

## Screenshots
#### Dashboard
![](screenshots/dashboard.png?raw=true)
#### Markdown Editor
![](screenshots/pages.png?raw=true)
#### SweetAlert
![](screenshots/sweetalert.png?raw=true)
#### File uploads
![](screenshots/files.png?raw=true)
#### Events
![](screenshots/events.png?raw=true)

## Installation

### Dependencies

Installation depends on `node`/`npm` with `grunt` and `bower` installed globally.

### Checkout this project:

    git clone https://github.com/beeman/loopback-angular-admin.git

### Install the Node packages:

    npm install

### Install the Bower packages:

    bower install

### Run a test to see if all is well:

    grunt

### Clone, install and run in a oneliner

    git clone https://github.com/beeman/loopback-angular-admin.git && cd loopback-angular-admin && npm install && bower install && API_URL=http://0.0.0.0:3000/api grunt && npm start & grunt serve

## Running

The project is separated in a server and a client.

### Server

To run the server you issue the command:

    npm start

Or to run it with nodemon (needs `nodemon` installed globally). This will
automatically restart the server when you change its code:

    npm run dev

### Client

Rebuild the lb-services.js file with the correct `API_URL` for development.

    API_URL=http://0.0.0.0:3000/api grunt

To run the client you issue the command:

    grunt serve

It will open the project in your default browser with livereload enabled.
This will take care of reloading the page when you change your code.

## Connect to a database

You can specify the URL to the MongoDB database you want to use with the `MONGODB_URL` environment variable.

    MONGODB_URL="mongodb://localhost:27017/loopback-angular-admin" npm start

Set `INITDB` to true if you want to load the initial dataset, which creates the admin user. The memory database (default) does this automatically.

    INITDB=true MONGODB_URL="mongodb://localhost:27017/loopback-angular-admin" npm start

This also works with the free hosted MongoDB instances at [compose.io](https://www.compose.io) and [mongolab.com](https://mongolab.com)!

## Development

For development you'd want to look into [yeoman](http://yeoman.io).

The API is built with [generator-loopback](https://www.npmjs.org/package/generator-loopback).

The GUI is built with [generator-angular](https://www.npmjs.org/package/generator-angular).

These should help you quickly add code to your project. Further details tailored to this project might follow in the future.

### Useful commits

These commits might be useful when extending the functionality.

- [Add support for MongoDB databases](https://github.com/beeman/loopback-angular-admin/commit/6b884e601d535ed64b4ef4f6f07e0f55d357a5b6)
- [Add custom method to the API](https://github.com/beeman/loopback-angular-admin/commit/eedbd03f755ddf2234872886ee390ac4f6753c64)
- [Add a complete model in the API and client](https://github.com/beeman/loopback-angular-admin/commit/16b1015554a41e45ca670d25fd258340908c4dbf)
- [Rename a model](https://github.com/beeman/loopback-angular-admin/commit/88254ce59af29818aec900514693e3fe6c94acea)

# Issues

If you have any problems please [contact me](https://github.com/beeman/loopback-angular-admin/issues/new).
