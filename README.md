---
description: In no particular order...
---

# Resources

### Things

* The [twelve factor app](https://12factor.net/) is a methodology used for building software as a service.
* A [great page](https://chris.beams.io/posts/git-commit/#seven-rules) describing 7 really good rules to follow when writing git commit messages.
* I use [draw.io](https://www.draw.io/) to draw diagrams to communicate architecture and other things to the team.
* A great collection of resources turned into handbook for the[ front-end developer](https://frontendmasters.com/books/front-end-handbook/2018/).
* A pdf diagram of the different [design patterns](http://www.mcdonaldland.info/files/designpatterns/designpatternscard.pdf).
* The [BFF/Companion pattern](https://samnewman.io/patterns/architectural/bff/) explained by Sam Newman.
* Read up on the difference between using [mock and stub](https://martinfowler.com/articles/mocksArentStubs.html) objects for testing. I believe the important difference between the two is that mocks verify behaviours and stubs verify state.
* Deeeeep server philosophy [Pets vs Cattle](https://www.engineyard.com/blog/pets-vs-cattle)
* Deeeeep architectural philosophy [microservices](https://martinfowler.com/articles/microservices.html)
* Presentation on [how to pair](https://community.rea-group.com/docs/DOC-62392-pairingpresopdf)
* Open Web Application Security Project \(OWASP\) has released the [top 10 application security risks](https://www.owasp.org/index.php/Top_10-2017_Top_10) as of 2017
* Internally we document and make decisions through an Interested Parties Review \(IPR\). What is an [IPR](https://community.rea-group.com/docs/DOC-47219-interested-parties-review)?
* There's a good book written by Robert C. Martin on what is clean code. A summary of that book can be found [here](https://gist.github.com/wojteklu/73c6914cc446146b8b533c0988cf8d29).
* A great list of computer science topics to get into your brain. [Teach yourself computer science](https://teachyourselfcs.com/)
* [Basic description](https://github.com/lichstars/party/blob/master/continous-delivery.md) of the difference between continuous integration, continuous delivery and continuous deployment.

### React

* [React](https://reactjs.org/docs/hello-world.html) is a javascript library for building interfaces for single page applications. The React official docs is amazing and a great place to start to learn all things React. They also offer a [tutorial](https://reactjs.org/tutorial/tutorial.html) that you can follow along with which I highly recommend if you are new to React.
* Alternatives to learning React are
  * [Codecademy course](https://www.codecademy.com/learn/react-101) for beginners
  * Beginners into to React on [egghead.io](https://egghead.io/courses/the-beginner-s-guide-to-react)
  * [Udemy course](https://www.udemy.com/react-redux/learn/v4/content) \(not free\)
  * [Pluralsight](https://app.pluralsight.com/library/courses/react-big-picture/table-of-contents) \(not free\)
  * React fundamentals with [TylerMcginnis.com](https://tylermcginnis.com/courses/react-fundamentals/) \(not free\)
* Common things/libraries that we use that you could focus your learning on
  * React [lifecycle methods](https://reactjs.org/docs/react-component.html) can be quite useful so it's good to know about them
  * For state management use [redux](https://redux.js.org/).  Such good [documentation](https://redux.js.org/introduction) on this library.
  * To connect your redux store with react there's a really simple library called [react-redux](https://github.com/reactjs/react-redux). This library comes with two api's `connect` and `Provider`. I really like this further explanation on react-redux's [connect](https://www.sohamkamani.com/blog/2017/03/31/react-redux-connect-explained/).
  * Forms. Building [react forms](https://reactjs.org/docs/forms.html) is easy, but if you want to connect them to your redux store, use [redux form](https://redux-form.com/7.3.0/docs/gettingstarted.md/).
  * For routing between pages in your app read up on using the [react router](https://reacttraining.com/react-router/core/guides/philosophy).
* Add redux dev tools to your [chrome extensions](https://github.com/zalmoxisus/redux-devtools-extension) to view react redux state in your browser, which can make testing things easier.
* We write most of our css code in react using the library [styled-components](https://github.com/styled-components/styled-components)
* We use create-react-app to speed up the delivery of our single page apps. It creates all the things we need to get started very quickly. It makes a lot of assumptions and hides all the configuration files. This is great for simple client side apps, but not so great if you want server side rendering.
  * What is [webpack](https://webpack.js.org/concepts/)
  * What is [create-react-app](https://github.com/facebook/create-react-app)
  * What is [server side rendering](https://medium.freecodecamp.org/demystifying-reacts-server-side-render-de335d408fe4)

### Javascript

* [Top 10 features you should know about ES6](https://webapplog.com/es6/)
* Sooner or later you're gonna hit a javascript thing known as a [Promise](https://scotch.io/tutorials/javascript-promises-for-dummies).
* [Babel ](https://babeljs.io/)is a JavaScript [transpiler](https://en.wikipedia.org/wiki/Source-to-source_compiler). What that means is that we can take ES6/[ES2015](https://babeljs.io/docs/learn-es2015/) code and make it work on all browsers, even ones that may not support it. Essentially Babel takes the ES6 JavaScript code and compiles it into ES5 code. Although all of the code is transpiled, there are still some things like Promises and new methods that aren't recognised. A polyfill such as [babel polyfill](https://babeljs.io/docs/usage/polyfill) will help with that.
* To make all our javascript code adhere to some styling standards we use [eslint](https://eslint.org/). Get it for your IDE.

### Docker

* Lynda.com has an amazing beginner's video tutorial on Docker and how it can be used.
* Here's a short 8 min youtube [video](https://www.youtube.com/watch?v=pGYAg7TMmp0) \(not sure of quality\)
* [Gett started & installation](https://docs.docker.com/get-started/#test-docker-installation)
* [Docker-compose](https://docs.docker.com/compose/overview/) for multi-container shiz.

### Node

* [Node](https://nodejs.org/) is built well to handle asynchronous JavaScript code to perform many asynchronous activities such as reading and writing to the file system, handling connections to database servers, or handling requests as a web server. We build a lot of our backends-for-frontends \([BFFs / Companions](https://samnewman.io/blog/2015/11/23/backends-for-frontends-a-microservice-pattern/)\) with Node.
* Here's a good document on [what is node](https://www.codecademy.com/articles/what-is-node).

### Package managers

* Know what a package manager is and used for. [NPM](https://docs.npmjs.com/getting-started/what-is-npm) and [Yarn](https://yarnpkg.com/en/) aren't the only two available but [here's a document](https://medium.com/@nikjohn/facebooks-yarn-vs-npm-is-yarn-really-better-1890b3ea6515) explaining the difference as a starting point. From the npm and yarn doco pages, a good thing to understand is [what a package is and what a module is.](https://docs.npmjs.com/getting-started/packages)

### Vesioning
* Making a change to one of our libraries? Learn about [semantic versioning](https://docs.npmjs.com/getting-started/semantic-versioning)
* A great standard on how to manage a [changelog](https://keepachangelog.com/en/1.0.0/). Probably good to implement on libraries so the team knows what changes they're pulling in.

### Testing

* Use [Charles](https://community.rea-group.com/docs/DOC-65919-testing-finx-in-native-apps-using-charles) to proxy requests so we can test on mobile devices. 
* If your react app was bootstrapped by create-react-app, you'll find it comes with Jest out of the box. [Jest](https://facebook.github.io/jest/docs/en/expect.html) is a test runner.
* [Enzyme](http://airbnb.io/enzyme/) is a JavaScript Testing utility for React that makes it easier to assert, manipulate, and traverse your React Components' output. 
* Incorporate the [sinon](http://sinonjs.org/) library when you need stubs/spies/mock/fakes.

### Git
* An interactive clickable Git [cheatsheet](http://ndpsoftware.com/git-cheatsheet.html)
* Never lose a commit again. [Recover lost git commits](http://effectif.com/git/recovering-lost-git-commits) and [using git reflog](https://www.atlassian.com/git/tutorials/rewriting-history/git-reflog).
* Keep [your fork up to date](https://gist.github.com/CristinaSolana/1885435)

### What's in the news
* https://news.ycombinator.com/

### For entertainment

* A basic starting point into learning about [Encryption](https://github.com/lichstars/party/blob/master/encryption.md)
* Read the [bitcoin paper](https://bitcoin.org/bitcoin.pdf)
* A relatively easy to understand primer on [elliptic curve cryptography](https://blog.cloudflare.com/a-relatively-easy-to-understand-primer-on-elliptic-curve-cryptography/)
* What is a [distributed hash table](https://en.wikipedia.org/wiki/Distributed_hash_table)
* What is [consistent hashing](https://en.wikipedia.org/wiki/Consistent_hashing)
* What is a [Merkle tree](https://en.wikipedia.org/wiki/Merkle_tree)
* What is the [CAP theorem](https://en.wikipedia.org/wiki/CAP_theorem)
* White paper on Amazons Distributed [Dynamo tech](https://www.allthingsdistributed.com/2007/10/amazons_dynamo.html)
