backbone-server
===============

Implements an in-memory server for Backbone.js
http://documentcloud.github.com/backbone/#Sync

This project is a teaching aid. It provides an out-of-the-box server that Backbone.js models can sync with.

It uses the [CORS headers](https://developer.mozilla.org/en/http_access_control) to allow cross-origin requests.

Usage
-----

1. Clone the repository

1. Install node.js

1. Install the dependencies with `npm install`

1. Start the server with `node rasterver.js`

1. Configure your models / collections with urls in the form `http://localhost:8080/[collectionname]`

Extras
------
I added following features apart from original Backbone server.

* Instead of having empty data, I added sample data javascript file(data.js) with sample collection.
  You can place your own collection in the file.
* Removed idCounter field. The id is created based on the collection length. 
* Updated port number from 3002 to 8080.

P.S.
----

For truly zero-config usage I run a hosted instance of backbone-server at http://withouttheloop.com:8080. Set your model's url to `http://withouttheloop.com:8080/[some unique collection id]` and it will work magically. I do occassionally restart the service so not recommended for production. ;)

