# net.curiousprogrammer/stats-clj

Exploring statistics with Clojure.

## Usage

### Tests

Run the project's tests (they'll fail until you edit them):

    $ bin/kaocha

See https://github.com/lambdaisland/kaocha#all-tools for more info.

### Packaging

Run the project's CI pipeline and build a JAR (this will fail until you edit the tests to pass):

    $ clojure -T:build ci

This will produce an updated `pom.xml` file with synchronized dependencies inside the `META-INF`
directory inside `target/classes` and the JAR in `target`. You can update the version (and SCM tag)
information in generated `pom.xml` by updating `build.clj`.

### Installation and deployment 

Install it locally (requires the `ci` task be run first):

    $ clojure -T:build install

Deploy it to Clojars -- needs `CLOJARS_USERNAME` and `CLOJARS_PASSWORD` environment
variables (requires the `ci` task be run first):

    $ clojure -T:build deploy

Your library will be deployed to net.curiousprogrammer/stats-clj on clojars.org by default.

## License

Copyright © 2022 Juraj Martinka
Distributed under the Eclipse Public License version 1.0.
