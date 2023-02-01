# sbt-source-dist

An attempt to prototype the code to produce source distributions for
[Apache Pekko](https://github.com/apache/incubator-pekko).

This will ultimately be refactored so it can be called as an sbt task.

* Some code comes from https://github.com/neva-dev/gitignore-file-filter
* Some of the code was converted from the original Java to Scala - partially via IntelliJ autoconversion - some of that code needs work - to better follow Scala norms
* Uses the .gitignore and some extra custom patterns to exclude files from the generated zip and tgz files
  * support for nested .gitignore files has not been retained (it can be added back if it is actually useful)
* Outputs to target/dist directory
* The `Main` class hard codes `val homeDirectory` - so anyone trying this out should adjust that to match their setup
