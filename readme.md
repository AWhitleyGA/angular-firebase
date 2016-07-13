# AngularFire
- Create and configure a Firebase back-end.
- Create a Javascript that communicates with a Firebase back-end.
- Explain the difference between HTTP and Websockets, and provide an advantage and disadvantage of each.
- Explain what AngularFire is and how it differs from Firebase.
- Deploy your app to Firebase Hosting.

## Framing

Up until this point, we've used Postgres and SQL to persist data. Today we'll be exploring an alternative: Firebase.

## Firebase

#### What Is Firebase?

Firebase is a cloud-based database service. Not only can we access it programmatically using code, but we can also interact with data via a graphical interface in the browser.

Unlike Postgres, Firebase is a NoSQL database. This means that information is not stored in tables and it does not make use of associations like `has_many` or `belongs_to`. Instead, information in a NoSQL database is stored in one big JSON tree. We will go more into what exactly it means to use a NoSQL database when we explore Javascript back-ends after Project 3.

#### Why Use Firebase?

It's fast.
* Firebase uses Websockets to maintain a constant, open connection between the client and the database. Rather than use a traditional call-and-return system of requests and responses like HTTP, the browser and server are constantly in communication with each other and are immediately aware of changes on either end. Using Firebase, we can establish three-way data binding in an Angular application between the controller, the browser and the database.

> If you're interested in learning more about Websockets, [start here](http://www.html5rocks.com/en/tutorials/websockets/basics/).

It's user friendly.
* Firebase's graphical interface means we only need to load up a browser in order to explore what we have in our database.

Perhaps the biggest selling point: multiple clients can easily use the same database/API.
* It's just a matter of including the proper credentials in your application.

There are lots of notable apps that use Firebase, including Shazam and NPR One. [There are plenty more](https://firebase.google.com/customers/).

## AngularFire

How can we connect our Angular application to Firebase? By using **AngularFire**.

AngularFire is a Javascript library created by Firebase. It provides us with an intuitive means of interacting with a database not unlike ActiveRecord or ngResource. We will be using the AngularFire library to access Firebase from Angular. We'll explore how to use it by building a todo app later on in this lesson but if you'd like to learn more, [the official documentation is a good place to start](https://github.com/firebase/angularfire).

## Walkthrough: A To-Do App

To demonstrate how to use Firebase and Angular together, let's create a simple todo app...

**[Click here](\todo.md)**

## You Do: Grumblr and Firebase

Now it's your turn. For the remainder of the lesson, you will be adding Firebase to Grumblr...

**[Click here](\grumblr.md)**

## Closing / Questions

## Resources

- [AngularFire Quickstart](https://www.firebase.com/docs/web/libraries/angular/quickstart.html).  - [Firebase examples](https://www.firebase.com/docs/web/examples.html)
- [Firebase Hosting](https://www.firebase.com/docs/hosting/quickstart.html)
- [Simple (ruby) Server](http://www.benjaminoakes.com/2013/09/13/ruby-simple-http-server-minimalist-rake/)
- [Controller as](http://www.johnpapa.net/angularjss-controller-as-and-the-vm-variable/)
- [And again](http://toddmotto.com/digging-into-angulars-controller-as-syntax/)
