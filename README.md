Webpack is a static module bundler for modern JavaScript applications. When webpack processes your application, it internally builds a dependency graph from one or more entry points and then combines every module your project needs into one or more bundles, which are static assets to serve your content from.

Webpack is a bundler
That means that due to ES6 feature “modules” where import & export play good role there we can use webpack to reduce down all our separate JS files to one single huge JS file written in ES5, which is easily consumable by modern browsers & not just JS but with the help of respective plugins we can also use minified versions of other styles & asset files too.

Alternatives of Webpack -
Grunt, Gulp

Grunt, Gulp vs Webpack:

Grunt & Gulp are task runner whereas
Webpack is module bundler:-

A task runner is basically a program which automate tasks like
-> compressing JS file, reducing SaaS file to CSS file, minifying files, etc.
A module bundler is a program which visits all modules of our application and creates the static asset of its dependencies & THEN performs the operation of task runner on it.

The development & production build files are different because in production we are more concerned about speed of page instead it’s detailed information & speed is guaranteed by minified JS file.

Placeholder in JS
Placeholders are basically the identification attached to name of build file generated. Following are the available placehiolders available:

- [query]
- [name]
- [id]
- [hash]
- [chunkhash]
- [contenthash]

publicPath:
Lets say we have 3 build files created after npm run build.
1.js 2.js 3.js
Lets say 1.js is the entry point specified so now 1.js will just know the names ONLY not the content of other two files. Now, webpack knows WHAT possibly it has to fetch next but from WHERE that is answered by publicPath property in config.

For dealing with webpack we need following 3 dev-deps:
Webpack
Webpack-cli
Webpack-dev-server

Webpack-dev-server will let us run the code using a dev-server but it will NOT show any build file but do exist & it exists in RAM as RAM is faster to access compared to accessing from disk

Webpack hot reloading:
Hot-reloading is the mechanism which let the updation may occur on the DOM without completely reloading the DOM.
Benefit of hot-reloading:-
As component will not reload hence any change in code will let us not loose the existing state
And only selective update in DOM makes updation more efficient
