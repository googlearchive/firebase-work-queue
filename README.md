firebase-work-queue
===================

An example of processing data using Firebase as a queuing system.

To run, first you'll need to download the Firebase node client:
    `curl https://cdn.firebase.com/v0/firebase-node.js > firebase-node.js`

Now you can start a worker like this:
    `node worker.js`

And you can start a work generator like this:
    `node generator.js`

You can start as many workers or generators as you like. The WorkQueue uses transactions to ensure that each job is only given to one worker.
