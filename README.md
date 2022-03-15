# MongoDB Installation Walkthrough

# mongoDB_install
Installing and setting up MongoDB

MongoDB is a fantastic, internationally used database system. We will be using it through our second unit.

In our terminal, enter the commands


```
brew install mongodb mongodb-community

```

If linux/ubunto users are getting any permission errors, simply add the Sudo (Super User Do) command before

```

sudo apt brew install mongo mongodb-community

```

If you got any errors there, please let a consultant know. Otherwise, you can
verify that MongoDB is working correctly by running one of the following
commands:

### macOS

Run `brew services list`. You should see `mongodb-community` with the word "started" to
the right of it.

### Ubuntu

Run `sudo systemctl status mongodb`. You should see a green circle and the words
"active (running)" somewhere in the output.

### On either OS

If the service appears to be running, type `mongo` and hit enter.

You should see something like this:

```
MongoDB shell version v4.2.0
connecting to: mongodb://127.0.0.1:27017
MongoDB server version: 4.2.0
```

possibly followed by some warnings/errors. Ignore these warnings/errors for now.
You should notice that your command prompt is gone, replaced with a `>`.
This means the MongoDB shell installed correctly. Press `Ctrl + c` to get back
to your terminal.


If there are any further errors, we may have to run

```

sudo apt update

sudo apt install -y mongodb

```

Please let your instructor know if you need to run these additional commands
