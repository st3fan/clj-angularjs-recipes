This is an example Clojure web application project that uses the Angular.js framework and Bootstrap. It's functionality is pretty minimal: it just grabs a list of recipes from [Recipe Puppy](http://www.recipepuppy.com/) and then displays those in a table. You can change the main ingredient to load different recipes.

The client side code for the web app is in `index.html` and `index.js`. The server side bits are in `core.clj` and `recipes.clj`. The first defines the routes and a very simple JSON API to retrieve recipes. The latter interfaces to the [Recipe Puppy API]() to retrieve recipes.

To run the app you need to have Leiningen 2.0 installed. Then simply run:

```
$ git clone https://github.com/st3fan/clj-angularjs-recipes.git
$ cd clj-angularjs-recipes
$ lein ring server-headless
```

The app should then be running at [http://localhost:3000](http://localhost:3000)
